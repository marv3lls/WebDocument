## Troubleshooting

### 3tene stops after displaying the logo while it is running.

>2019/01/18 Fixed a startup bug caused by face tracking.
>2019/04/12 Fixed a startup bug caused by recording equipment.

>Try the latest 3tene.


### 3tene crashes during startup.

>2019/08/09 Introduced a countermeasure for the problem of forced termination due to the video save function.

>If you start 3tene while holding down the alt key, the video save function may be disabled and start.
>If it starts, go to the folder where you installed 3tene.
> If you create "Video Disable.txt" or "DisableMovie.txt" (the contents are empty)
> The video save function is always disabled.

> If you want to save the video, please install OBS separately and record 3tene.


### I get an error while starting 3tene.

>2020/06/30 Corrected.

>Try the latest 3tene.

>If &quot;Initialize Setting Error !!&quot; is displayed during startup
>It may be improved by clearing all the settings with
>Settings → System → Reset all settings


### 3tene (Pro version) is killed during startup.

>It seems that it may happen when the operation of SteamVR is unstable.
>Please close SteamVR and start it with the VR device disconnected (recognition).


### On Mac, the developer is displayed as unconfirmed and 3tene cannot be started.

>The action depends on the version of MacOS.

><font color="Blue">・10.15.x Catalina Common Workaround (2 Macs required)</font>
>Download 3tene and unzip it on a Mac that isn&#39;t Catalina.
>Recompress the unzipped and created folder into a zip.
>Copy the recompressed zip file to a Catalina Mac with a USB stick and unzip it.
>Run 3tene.

><font color="Blue">・10.15.2 Catalina</font>
>The coping method has not been established.

><font color="Blue">・10.15.1 Catalina</font>
>We have not confirmed.

><font color="Blue">・10.15 Catalina</font>
>Enter the following from the terminal.
>sudo spctl --master-disable
>When you execute it, you will be asked to enter the password, so enter it.
> Select &quot;System Preferences&quot; from the &quot;Apple&quot; menu on the top menu.
> Select &quot;Security &amp; Privacy&quot; and select the &quot;General&quot; tab.
> Click &quot;Lock&quot; at the bottom left and enter the password.
> Select &quot;Allow all applications&quot;. Execute
> 3tene.

> · 10.14.x Mojave and earlier
> Control-click the 3tene icon.
> &quot;Open&quot; forcibly starts.

### Face tracking doesn&#39;t work! (3tene ver 1 series)

>Did you press the start button for face tracking on the right menu?
>It turns green during operation.
><font color="Red">* In many cases, you forget to press it.</font>

>![image](image/menu_face.png "Face recognition ON")

>Also, make sure you have specified the webcam you want to use to adjust your avatar.
>確認方法は[こちら](#ft_webcamera.md)を参照してください。


### フェイストラッキングの開始ボタンが無効状態で押せません！

>2020/08/04 修正を行いました。

>最新の 3tene を試してみてください。

>3tene が VRM の読み込みに失敗すると発生します。

>VCランタイム 2015-2019 (x64) をインストールすると改善する可能性があります。
><a href="https://support.microsoft.com/ja-jp/help/2977003/the-latest-supported-visual-c-downloads" target="_blank">Visual C++ 再頒布可能パッケージ 2015-2019</a>より vc_redist.x64.exe をダウンロードしてください。


### 以前は動作していたのにフェイストラッキングが動作しなくなりました

>USB接続のウェブカメラを使用していませんか？
>前回使用していたウェブカメラを取り外している状態で 3tene を起動し、
><font color="Blue">後から前回使用していたウェブカメラを接続しても自動的には切り替わりません。</font>
><font color="Red">※Mac ではこれが原因で CamTwist が選択され強制終了する</font>事があるようです。

>3tene のウェブカメラ指定が変更されていないか確認してください。
>アバター調整 → 設定タブ → ウェブカメラ


### Windows でフェイストラッキングを開始すると失敗（もしくは強制終了）されます。

>「フェイストラッキングの初期化に失敗しました。」と表示される場合は下記条件で失敗するようです。
><font color="Red">※3tene のインスト－ルパスに全角文字があると失敗します。</font>
><font color="Red">※アカウント名に全角文字があると失敗します。</font>

>3tene の初期化パスの設定を変更すると改善する可能性があります。
>3tene の設定 → システム → 初期化パスを変更してください。

><font color="Red">※RealSense 接続前に 3tene を起動して Nuitrack を使おうとしても失敗します。</font>
><font color="Red">※「Logi Capture」等の仮想カメラを選択していても失敗します。</font>

>ウェブカメラの選択は[こちら](#ft_webcamera.md)を参照してください。


### Mac でフェイストラッキングを開始すると失敗（もしくは強制終了）されます。

>3tene にカメラやマイクの使用権限が無い場合に強制終了してしまいます。
>また、<font color="Red">「CamTwist」等の仮想カメラを選択していても失敗します。</font>

>Mac の「システム環境設定」を選択して、「セキュリティとプライバシー」をクリック、
>「プライバシー」をクリックする。「カメラ」を選択する。
>リップシンクを使う場合は「マイク」の使用も許可してください。


### フェイストラッキングの開始でカメラ起動がタイムアウトします。

>Windows 10 バージョン 1803 以降および Mac を使用している場合は
>3teneに対してカメラ使用を許可しないとタイムアウトします。
>OS のセキュリティ機能で 3tene にカメラの使用を許可してください。

>Windows10 (バージョン 1803,1809) の場合
>設定 → プライバシー → カメラ でアプリの設定を変更してください。

>Windows10 (バージョン 1903 以降) の場合
>設定 → プライバシー → カメラ でデスクトップアプリ設定（全体）を変更してください。

>Mac の場合
>「システム環境設定」を選択して、「セキュリティとプライバシー」をクリック、
>「プライバシー」をクリックする。「カメラ」を選択する。
>リップシンクを使う場合は「マイク」の使用も許可してください。

>さらにセキュリティソフトをインストールしている場合には
>セキュリティソフトによってカメラがガードされている場合もありますので
>セキュリティソフトの設定も確認してください。

>また、画面更新が停止しているウェブカメラを選択すると開始に失敗します。
>対象となるカメラの画面更新が行われるようにするか、
>3teneのアバターの調整「設定」で使用するウェブカメラを変更してください。

>Mac のウェブカメラ起動時間は長い為、タイムアウトする事が多いようです。
>3tene → アバターの調整 → 設定 で待ち時間を長く設定してください。
><font color="Blue">※最近の Mac で発生する事が多いようです。</font>

>MacBook で BootCamp を使用して起動した Windows 上の
>FaceTime HD Camera は解像度の問題で使用できないようです。


### Windows でウェブカメラを２つ接続しましたがどちらか片方しか動作しません。

>下記のデバイスの組み合わせで同時使用が出来ないのを確認しています。
><font color="Red">※ウェブカメラが標準ドライバで動作していると同時に使用できない可能性があります。</font>

>BUFFALO BSW20K07H (デバイス名：PC Camara → 標準ドライバ)
>BUFFALO BSW200MBK (デバイス名：USB_Camera → 標準ドライバ)

>メーカーから専用ドライバが配布されている場合はそちらを試してみてください。
>ドライバの変更は自己責任となりますのでご注意ください。

><font color="Red">ウェブカメラの同時使用については[こちら](#DeviceWebCamera.md)を参照してください。</font>


### フェイストラッキングを使うとモデルの頭が回転します。

>2019/03/29 顔が回転してしまう不具合を修正。
>2019/08/09 再度修正を行いました。
>最新の 3tene を試してみてください。


### iPhoneX にインストールした 3teneFT と接続できません。

>下記の２点を確認してください。
>・iPhoneX と PC が同じルーターに接続されている。
>・3tene (PC) セキュリティソフトでファイウォールが適切に設定されている。

><font color="Red">特にファイルウォールの設定を行っていないケースが多いです。</font>

>接続方法については[こちら](#ft_iphone.md)を参照してください。


### iPhoneX にインストールした 3teneFT がプチフリーズします。

>2020/02/14 3teneFT v1.1.0 にて修正を行いました。
>3tene 本体も v1.10.20 2020/02/14 以降を使用する必要があります。

><S>数十秒待つと復帰します。
>GPU 負荷で端末が一時的に停止してしまうようです。</S>


### ウェブカメラのプレビュー fps が極端に落ちる場合があります。

>部屋の明るさが極端に明るかったり、暗かったりすると
>ウェブカメラ内蔵の補正機能が働き、性能が極端に落ちる製品があります。
>明るさが一定に保てる場所に移動してみてください。


### リップシンクの設定で録音デバイスを認識していません。

>新しい Windows10 で本体のミニプラグ端子にマイクを接続して使用する場合は
>マイクをミニプラグに刺していないと録音デバイスを認識しない仕様になったようです。
>3tene でミニプラグ接続のマイクを使用する場合は常に接続しているようにしてください。


### リップシンクを音声認識に設定して開始すると失敗します。

>アバターの調整 → 設定から「リップシンク起動待ち時間」を長くしてみてください。
><font color="Blue">※最近の Mac で発生する事が多いようです。</font>


### リップシンクを音声認識に設定して開始しても反応しません。

>OS (Windows,Mac) の録音機器に関連する音量やミュートの設定を確認してください。
>複数の録音機器が接続されている場合には
>アバターの調整 → 設定から「リップシンクの音声入力」が
>使用したい録音機器になっているかを確認してください。


### LeapMotion が動作しません。

>LeapMotion の動作には専用ソフトウェア(Ver 4 系)のインストールが必要となります。
>専用ソフトは公式サイトよりダウンロードしてください。
>Orion Ver 4.0.0+52173 で動作するのを確認しています。

>専用ソフトウェアのインストール後に 3tene を起動します。
>3tene → アバターの調整 → 設定タブ → 操作方法を「LeapMotion」に変更します。


### LeapMotion の鏡の動作が正しく反映されません。

>今後、修正を行う予定です。


### Perception Neuron が動作しません。

>別途、Axis Neuron (PRO) のインストールが必要です。

>Axis Neuron を起動して設定変更を行う。
>　※Settingsの「Broadcating」タブを選択し、「BVH」の「Enable」を選択する。
>Axis Neuron で Perception Neuron のハブに接続を行う。
>Axis Neuron で Perception Neuron のキャリブレーションを行う。
>Axis Neuron を起動したまま 3tene を起動します。
>3tene → アバターの調整 → 設定 → 操作方法を「PerceptionNeuron」に変更します。

>[Perception Neuronについて](#PerceptionNeuron.md)


### VR が動作しません。

>別途、SteamVR のインストールが必要です。

>SteamVR のインストール後に 3tene を起動します。
>3tene → アバターの調整 → 設定 → 操作方法を「VR」に変更します。
>3tene → 設定 → VR → ゴーグルやトラッカーの部位設定を行います。


### HTC Vive から HTC Vive Pro に交換したら動きません。

>SteamVR が極端に古い場合はアップデートが必要です。

>アップグレード版でゴーグルとリンクボックスを交換した場合は
>コントローラの再ペアリングをする必要があります。

>フルセット版の場合はペアリングとルームの再設定が必要です。


### RealSense + Nuitrack が動作せず、プレビューが真っ白です。

>アクティベーションが完了していないか他のソフトと競合しています。
>[こちら](#Nuitrack.md) で手順を確認してください。


### 動画保存を行うと音声が記録されません。

>仕様となります。
>音声も記録したい場合は OBS の使用をお勧めします。


### Windows で 3tene の画面が OBS に正しく表示されません。

>3tene v1.10.20 2020/02/14 以降ではウインドウキャプチャではなく
>ゲームキャプチャからウインドウを指定するようにしてください。
>（Mac 版はウインドウキャプチャを使用してください。）

>なお、OBS との連携では[仮想ウェブカメラ](#VirtualWebCamera.md)を経由した
>映像キャプチャデバイスによる使用が推奨されます。
>メニューやウインドウを表示したい場合はゲームキャプチャを使用してください。


### Mac で OBS のウインドウキャプチャ表示ができません。

>macOS Catalina (10.15.x) はセキュリティが厳しくなっていますので、
>初期状態ではOBSのウインドウキャプチャが使えない場合があります。

>[システム環境設定] -> [セキュリティとプライバシー] -> [プライバシー] -> [画面収録]
>に OBS が無い場合、および OBS にチェック付いてない場合が該当します。

>OBSで「空の名前でウインドウを表示」にチェックすると、一覧に項目が追加されます。
>追加された項目を選択すると「画面収録」の許可を求められるので
>許可すると一覧に 3tene が現れので選択します。


### VRoid Studio で作成したアバターの表示が崩れる場合があります。

>複雑な頂点構成のアバターで発生する事があるようです。
>設定「システム」タブでクオリティを「Very High」以上に変更してみてください。
>改善される場合があります。
>ただし、処理負荷が増えるのでパフォーマンスは低下します。

>![画像](image/quality_vroid.png "クオリティ")
><font color="Blue">※VRoid Studio でパーカーを使用している場合。</font>


### 自作した VRM の表情を変更すると目や口が２重に表示されてしまいます。

>3tene では VR に対応している為、VRM は First Person に対応している必要があります。
>VRM を First Person に対応させるか、「Third Person Only」に設定変更を行い、
>First Person を無効にしてください。


### アバターの頭や顔のパーツが描画されません。

>シーンカメラがアバターに近いと発生するようです。
>DirectX 11 に対応している GPU (内蔵グラフィック) だと発生しないようです。

>2019/03/14 強制描画を行うオプションを追加しました。（標準でON）
>最新の 3tene を試してみてください。


### Intel Core 2000 番台の内蔵グラフィックを使用していますが描画が崩れる事があります。

>Intel Core 2000 番台に搭載されている GPU (内蔵グラフィック) は対象外となります。

>Intel Core シリーズの内蔵グラフィックを使用する場合は 4000 番台以降が対応となります。
>※MacBook (Pro, Air 含む) 2011、2012 は対象外となります。

>デスクトップPCであればグラフィックボード(GPU) を追加する事で改善される可能性はありますが、
>グラフィックボードの追加および交換は自己責任となります。
><font color="Blue">※DirectX 11 以降に対応したグラフィックボードを使用してください。</font>

>[動作環境](#required.md)


### 背景のウェブカメラに仮想ウェブカメラを指定すると黒画面表示になります。

>仮想ウェブカメラソフトによって挙動が異なるようです。
>LogiCapture の場合は 3tene で背景ウェブカメラを LogiCapture で開始した後に
>本体の LogiCapture を起動すると正常表示するのを確認しています。
>LogiCapture を先に起動していると黒画面になるのを確認しています。


### ショートカットの左手、右手が動作しません

>全身トラッキング中(VR, Nuitrack, Perception Neuron)のみ動作します。

>Perception Neuron の場合はアバター調整の「設定」→「全ての指を制御する」の
>チェックを外していないと手の形状は変化しません。

>ショートカットの[注意事項](#settingShortcut.md)


### オブジェクトの読み込みで失敗します。

>読み込みたいオブジェクトのファイルパスに日本語のフォルダが
>入っていると失敗します。
>日本語が含まれないパスにファイルを移動してから読み込みを行ってください。


### 3tene を非アクティブにしてしばらくすると画面更新が止まったりチラツキます。

>2019/04/18 チラツキの対策を行いました。
>最新の 3tene を試してみてください。
