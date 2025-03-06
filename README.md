
<!DOCTYPE html>
<html lang="vi">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Tỏ Tình</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #ffe6e6;
        }
        .container {
            margin-top: 100px;
        }
        h1 {
            color: #ff4d4d;
        }
        .btn {
            font-size: 20px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        .yes {
            background-color: #ff4d4d;
            color: white;
        }
        .no {
            background-color: #666;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1> tui thích bạn á,bạn có thích tui hông^^?💖</h1>
        <button class="btn yes" onclick="acceptLove()">CÓ</button>
        <button class="btn no" onmouseover="moveNoButton()">hông</button>
    </div>
    <script>
        function acceptLove() {
            document.body.innerHTML = '<h1>Yay! tôi bt mà=)) 💕</h1>';
        }
        function moveNoButton() {
            let button = document.querySelector('.no');
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            button.style.left = `${x}px`;
            button.style.top = `${y}px`;
        }
    </script>
</body>
</html>
