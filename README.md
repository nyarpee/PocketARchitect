Androidのみの対応です。
motorola x40以外のスマホにUIの最適化を行っていないのでUIの位置がずれると思います。（今後アップデートします。）
apkをインストールしようとすると不明元からの...とエラーが表示されると思いますが、提供元不明のアプリのインストールを許可する事でインストールできます。
わからないことがあればfcuapps@gmail.comに連絡ください。

#基本的な使い方
アプリの機能を生かすには平面を検出してもらう必要があります。
地面もしくは平面に対してスマホを平行に配置し動かすと平面が検出されやすいです。（検出された場合ドットが現れます。）
平面が検出されるている場所にはレーティクルが表示されます。
フッターにある丸いボタンを押すことでオブジェクトを配置したりできます。

各モードについて説明します。

##PlaceObject
文字通りオブジェクトを検出した平面上に置くことができます。
上の三からオブジェクトを選んで配置してください。（フッターのボタンを押すとレーティクルの中心に配置されます。）
レーティクルを配置されているオブジェクトの上に持っていくとアウトラインが表示されその状態で再度ボタンをおすと編集モードへと入ります。
編集モードではオブジェクトの大きさ、回転を変更することができます。
二本指のピンチでサイズの調整。
一本指でスワイプで回転の調整。
インプットフィールドに大きさを入力するとより細かくサイズを調整できます。（unitを押すことでｍ、ｃｍ単位を切り替えれます。）

##Mesure
距離の測定や空間の測定に役立ちます。
操作が複雑なのですが基本的なプログラムとしては球体と球体の間の距離を計測しています。
なので球体をユーザーにおいてもらう必要があります。
上下に画面をスワイプすることで球体を配置する方法を切り替えられます。
o-oのマークのContinuousModeを使うことで自動的に点と線を繋いでくれます。（これ以上球体を配置する必要がない場合一つ前の球体に接続してください。）
↑マークのyaxisModeを使うことで縦方向に球体を配置することができます。すでに配置しているオブジェクトの上でボタンを押すとそのオブジェクトをy方向に複製してくれます。（青色の↑マークはすべての球体をｙ方向に複製します。黒色は一つの球体を複製します。）

editボタンを押すことで球体の位置を変更したりどの球体とどの球体を接続するかを編集できます。editモードで球体上で一本指の長押しで球体を選択します。
（青のアウトラインは現在選択している球体、赤のアウトラインは現在選択している球体から線でつながっている球体。赤の球体上で一本指の長押しで接続の解除。もしくは一本指のスワイプで球体の移動ができます。）
lengthボタンを押すとつながっている線上に距離が表示されます。
angleボタンを押すと角度が表示されます。（二つ以上の線が球体から出ているときのみ）

##LoadFile
セーブ済みのデータが表示されます。
セーブを行うにはPlaceObjecもしくはMesureモード上のヘッダー内にあるsaveボタンを押し表示されるインプットフィールドに名前を入力しセーブすることができます。
セーブしたコンテンツのロードボタンを押すことで以前セーブした環境を再現する事ができます。（位置がずれることがあるのでPlaceObject,Mesureモードのヘッダーにある移動モードを押すことで全体を移動することができます。）
ただしセーブデータをロードする際現在の環境はすべてリセットされてしまいます。

##Map機能について
丸いボタンの右にあるMapボタンを押すことで現在表示されているオブジェクトを三人称視点で確認することができます。

##オブジェクトのインポートについて
オブジェクトをインポートしたい場合は.obj形式のファイルをandroid>data>com.DefaultCompany.PlaneDetectionDemo>files>ObjectModelの中に手動で追加する必要があります。
追加後アプリを再起動するとインポートされます。

