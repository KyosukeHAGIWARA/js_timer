# README

### create at 2018/10/15
### update at 2018/10/15

## Description
HTMLの要素をタイマーで切り替えるjsスクリプトです。

## Usage
1. スクリプトファイルをディレクトリに配置
    + [view_timer.js](https://github.com/KyosukeHAGIWARA/js_timer/blob/master/view_timer.js)
    + ファイル名は `view_timer.js` から変更不可
1. 本体ファイルにimport

    ```HTML
    <!--head内で-->
    <script src="https://ajax.googleapis.com/ajax/libs/jquery/2.1.3/jquery.min.js"></script>
    <script src="./view_timer.js"></script>
    ```
1. 対象elementに　`class` 名 `view_timer` と、 `data-start-date` もしくは `data-end-date` 属性を付与

    ```HTML
    <!--設定時刻で表示を消す場合-->
    <span class="view_timer" data-end-date="2018/10/15 12:29">
        <a href="https://www.google.com" target="_blank">
           <img src="hoge.png" alt="2018/10/15 12:29 でこの要素は消えます" />
        </a>
    </span>    

    <!--設定時刻から表示させる場合-->
    <span class="view_timer" data-start-date="2018/10/15 12:29">
        <a href="https://www.google.com" target="_blank">
           <img src="hoge.png" alt="2018/10/15 12:29 からこの要素は出現します" />
        </a>
    </span>
    ```
    
## Tips
1. 要素切り替えの場合は上のように終了と開始を並べるとできます。
    + `data-end-date` と `data-start-date` の時刻が同じでも問題なく切り替えが起こります
    
## License
MIT

## Ask
hagiwara-ky [at] rittor-music.co.jp