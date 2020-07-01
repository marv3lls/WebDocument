## Azure Kinect について

>深度カメラによってボディトラッキングを行います。


### Azure Kinect の要求スペック

>Azure Kinect でボディトラッキングを使用する為には高性能PCが必要になります。

>・ＣＰＵ：第7世代 Core i5 クアッドコア 2.4GHz 以上
>・メモリ：4GB 以上
>・ＧＰＵ：NVIDIA GeForce GTX 1070 以上
>・接続：USB 3.x 必須。（USB 2.0 では Kinect を認識しません。）

>Azure Kinect は <font color="Red">CUDA を使用するので NVIDIA 製 GeForce シリーズが必須となります。</font>
>Intel の ＣＰＵ内蔵グラフィック、および AMD 製の Radeon シリーズには対応していません。

><a href="https://docs.microsoft.com/ja-jp/azure/kinect-dk/system-requirements" target="_blank">公式：Azure Kinect 要求機能（英語）</a>

>「Visual Studio 2015 の Visual C++ 再頒布可能パッケージ」のインストールが別途必要です。
><a href="https://docs.microsoft.com/ja-jp/azure/kinect-dk/body-sdk-setup" target="_blank">公式：開発者向けクイックスタート</a>


### 注意事項

>・黒い衣服を着ていると認識率が低下します。
>・現在のバージョンは複数人の認識に対応していません。（必ず１人だけ写るようにしてください。）


### 3teneKinect について

>3tene(PRO, STUDIO) で Azure Kinect を使用する為には
><font color="Blue">別途 3teneKinect が起動している必要があります。</font>

>3teneKinect が Azure Kinect の制御を行い、
>その認識結果を 3tene 側で受け取り、アバターに動きを反映させます。

>3teneKinect は AzureKinect DK の Sensor-SDK 1.3.0、 BodyTracking-SDK 1.0.1 を使用して
>作成されています。
>認識する部位は頭、腕、手、腰、足となりますが指は親指と人差し指のみとなります。
>指の認識ではブレが発生しやすい為、3teneKinect では指の制御機能を用意しています。


><font color="Red">3teneKinect</font> の<a href="https://3tene.com/pro/" target="_blank">ダウンロード</a>

>PC 1台で構成する場合は下記になります。
>![画像](image/kinect_howto_1.png "")

>Azure Kinect 用の高性能 PC を別途用意する事で負荷分散も行えます。
><font color="Red">※β版で分散機能は提供されません。</font>
>![画像](image/kinect_howto_2.png "")


### Azure Kinect の操作手順

>1. 3tene を起動する。
>2. 3teneKinect を起動する。
>3. 3teneKinect で Azure Kinect の制御を開始する。
>![画像](image/AzureKinect_1.png "")
>4. 3tene でボディトラッキングを Azure Kinect に設定します。
>![画像](image/AzureKinect_2.png "")
>5. 3tene のトラッキングを開始します。
>![画像](image/AzureKinect_3.png "")



