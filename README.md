leap_arduino
============

LEAP MOTION x Arduino Robot


-----

サーバーインストール・起動

    python 2.7.5 をインストール
    $ cd leap_arduino
    $ npm install
    $ node app.js

----- 

ロボットの作成・スケッチのインストール

    Arduino UNO に Ardumotoをスタックし、それぞれのモーター出力ポートに左右のモーターをそれぞれ取り付ける。
    戦車の本体はタミヤのタンク工作基本セット等で構築する
    USB で PC と接続し、leap_arduino/arduino/leap_arduino_sketch/leap_arduino_sketch.ino を書き込む
    
----- 

プログラムの実行
    
    LEAP MOTION を PC に接続
    ブラウザで http://localhost:3000 にアクセスする
    手を LEAP MOTION に認識させて次の通り操作する
      1. 認識される手の位置が画面右側 ==> 右旋回 
      2. 認識される手の位置が画面左側 ==> 左旋回 
      3. 認識される指の本数が "5" 本 ==> 前進
      4. 認識される指の本数が "2" 本 ==> 後退 
      5. 認識される指の本数が "0" 本 ==> 停止 
