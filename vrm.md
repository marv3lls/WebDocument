## VRMについて

### VRMとは？

>3Dアバター向け汎用規格「VRM（Virtual Railroad Models）」の事で、
>ドワンゴ株式会社から2018年4月に発表されました。

>VRM は Khronos グループによって策定された汎用3Dフォーマット「glTF 2.0」を拡張して
>VRソフトウェアや VTuber 配信に最適化したフォーマットです。

><font color="Blue">人型に限定する事によりアバターを扱うソフトウェアで高い互換性を維持しています。</font>

>※Khronos は「OpenGL」や「Vulkan」等、３Ｄ技術を策定する非営利団体の技術コンソーシアムです。


### どうすれば VRM を作れる？

>Unity に VRM の公式サイトよりダウンロードしたアセットを追加し、
>作成済みのモデルデータ（FBX等）を取り込んで調整を行い、
>VRM に変換するのが基本となりますが難易度が高かったりします。

>最近ではモデリングソフトでも対応しているものが少しずつ増えているようです。

>無料のモデリングソフト Blender は追加プラグインによって
>VRMのインポートが可能になっています。
>VRM を作成する場合は FBX で出力を行い Unity で VRM に変換します。

>また、プロに使われているモデリングソフト MAYA も
>VRM のエクスポートに対応するプラグインがあります。
>※VRM のインポートには対応していません。


### 3tene で使用する VRM を作る場合の注意点は？

>VRM を作成する場合の注意点を記載します。

>#### VRoidStudio で作成した VRM について
>VRoidStudio で作成した VRM を 3tene で読み込むのは問題ありませんが、
>VRoidStudio で作成した VRM を unity にインポートすると
>目のボーンの設定値が変化してしまい、目の移動範囲が狭くなります。
><font color="Blue">VRM へのエクスポート前に目の修正が必要になります。</font>

>また一部の服装で描画崩れが発生する場合は 3tene の
>設定「システム」タブでクオリティを「Very High」以上に変更してみてください。


>#### First Person について
>3tene では VR に対応している為、VRM は First Person に対応している必要があります。
>対応していないと目、まぶた、口が２重に表示されるといった現象が発生します。

>VRM を First Person に対応させるか、該当する顔の部位に
>「Third Person Only」に設定変更を行って First Person を無効にしてください。
><font color="Blue">※First Person を無効にすると VR 使用時の描画に問題が発生します。</font>


### VRM の仕様は？

>下記のサイトより Unity 用のアセット入手や技術仕様の参照が可能です。

>VRM の公式サイト
>日本語：<a href="https://vrm.dev/" target="_blank">https://vrm.dev/</a>
>英語：<a href="https://vrm.dev/en/" target="_blank">https://vrm.dev/en/</a>

>VRM の技術仕様 (glTF 2.0 との差異および拡張仕様)
><a href="https://github.com/vrm-c/vrm-specification/blob/master/specification/0.0/README.ja.md" target="_blank">日本語</a>　<a href="https://github.com/vrm-c/vrm-specification/blob/master/specification/0.0/README.md" target="_blank">英語</a>


