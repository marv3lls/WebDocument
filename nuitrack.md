## Nuitrack について

>深度カメラの骨格認識によって全身を操作します。

### 注意事項

>・黒い衣服を着ていると認識率が低下します。
>・Nuitrack のフェイストラッキングも同時に使用している場合に
>　全身を認識する距離まで離れると顔が認識できなくなる可能性が高いです。

### RealSenseの設定

>公式ホームページは<a href="https://www.intel.co.jp/content/www/jp/ja/architecture-and-technology/realsense-overview.html" target="_blank">こちら</a>

>SDKダウンロードページは<a href="https://www.intelrealsense.com/sdk-2/" target="_blank">こちら</a>

>SDKダウンロードページの「Download SDK for Windows 10」をクリック

<img src = "image/RealSense1.jpg" width = 70%>

>Intel.RealSense.SDK.exe のダウンロードが完了したら実行してインストールします。


### Nuitrackの設定

>公式ホームページは<a href="https://nuitrack.com/" target="_blank">こちら</a>

>ライセンスの購入（ライセンス購入前にトライアルにて動作確認を推奨します。）

>以下の設定の公式マニュアルは<a href="http://download.3divi.com/Nuitrack/doc/Installation_page.html" target="_blank">こちら</a>

>1. nuitrack-windows-x86.exe（Windows 32ビットの場合）またはnuitrack-windows-x64.exe のダウンロード、インストール
>nuitrack-windows-x86.exe（Windows 32ビットの場合）またはnuitrack-windows-x64.exe（Windows 64ビットの場合）を ダウンロードして実行します。
>「Windows によって PC が保護されました」と表示された場合は、詳細情報 → 実行 をクリックします。

>2. Microsoft Visual C ++ Redistributableをインストール（公式マニュアルの3のリンクから）

>3. システム環境変数が自動設定されていない場合は手動で設定
>コントロールパネル – システムとセキュリティ – システム – システムの詳細設定 – 環境変数 を開く

>>システム環境変数 – 新規 を開き、
>>変数名：NUITRACK_HOME
>>変数値：nuitrack-win64/nuitrackのパス
>>※標準インスト－ルした場合は下記のパスを入力してください。
>>C:\Program Files\Nuitrack\nuitrack\nuitrack

>>システム環境変数 – Path（変数名）を選択 – 編集 – 新規 を開き
>>nuitrack-win64/nuitrack/binのパス
>>※標準インスト－ルした場合は下記のパスを入力して追加してください。
>>C:\Program Files\Nuitrack\nuitrack\nuitrack\bin

>4. アクティベーション
>RealSense USB 3.0以上で接続する
>C:\Program Files\Nuitrack\nuitrack\nuitrack\activation_tool\Nuitrack.exe（デフォルトの場合）
>を管理者として実行（右クリック - 管理者として実行）
>Compatibility test をクリック
>Compatibility test が完了したら 「Enter Activation Key」に Activation Keyを入力し「Activate」をクリック
>（Trial版の場合 Activation Key は "license"から始まる文字列になります。）
>アクティベーションに成功すると下部に「Activation complete!」と表示される。

### Nuitrack の動作確認

>Nuitrack をインストールしたフォルダにあるサンプルプログラムで動作を確認してください。
><font color="Red">サンプルプログラムと 3tene を同時に起動すると競合してしまう</font>ので
>正常に動作する事が出来たら必ず<font color="Blue">サンプルプログラムを終了した後に 3tene を起動します。</font>

>正常に動作しない場合は Nuitrack に関係するソフトウェアを全て終了した後に
>RealSence の USB 端子を抜き差しすると改善する場合があります。


### Nuitrackによるフェイストラッキングの設定

>Nuitrackによるフェイストラッキングをご利用の際はお手数をお掛け致しますが、下記の手順を行ってください。

>Nuitrackのデフォルトの設定では、Nuitrackのフェイストラッキングはオフになっています。
>nuitrack\data\nuitrack.config
>上記ファイルを開き、「Faces.ToUse」と「DepthProvider.Depth2ColorRegistration」をtrueへ変更してください。


### Nuitrack が正常に動作しない場合

>#### 3tene の Nuitrack プレビューが真っ白になる

>1. Nuitrack アクティベーションが完了していない可能性があります。
>トライアルコードもしくは製品コードでアクティベーションが完了後に
>再度、3tene を起動して試してみてください。

>2. 他の Nuitrack を使用するソフトと競合している可能性があります。
>他のソフトを終了後、 RealSence の USB 接続を外して、再度接続後に
>3tene を起動してみてください。


