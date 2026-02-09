<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <title>円のアニメーション</title>
    <style>
        /* 背景の設定 */
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            align-items: center; /* 垂直方向の中央 */
            background-color: #f0f0f0;
            overflow: hidden; /* 画面外に出た円を隠す */
        }

        /* 円のスタイル */
        .circle {
            width: 50px;
            height: 50px;
            background-color: #3498db;
            border-radius: 50%; /* 正方形を円にする */
            position: absolute;
            
            /* アニメーションの設定 */
            animation: move-right 3s linear infinite;
        }

        /* 右へ流れる動きの定義 */
        @keyframes move-right {
            0% {
                left: -60px; /* 画面の左外からスタート */
            }
            100% {
                left: 100%; /* 画面の右端まで移動 */
            }
        }
    </style>
</head>
<body>

    <div class="circle"></div>

</body>
</html>
