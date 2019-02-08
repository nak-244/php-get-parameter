# php-get-parameter
パラメーターの値を取得して条件分岐

## 活用方法
メールDMからホームページにきた人にだけCTAを表示させる（最初の１ページ目のみ）  

例えば、以下のURLでページに来た人にだけ表示、それ以外の人には表示させない。  

  https://cestlaview.com?utm_campaign=test01

## php記述例

    <?php
    //パラメータ（GET）の値を取得して$paramに代入
    $param = $_GET["utm_campaign"];

    //$paramがtest01だった表示"
    if ( $param == "test01" ) {
        echo '表示させたい内容（ソースを記述）';
    }
    ?>
