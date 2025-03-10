<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Special Question ❤</title>
    <style>
        body {
            text-align: center;
            font-family: Arial, sans-serif;
            background-color: #ffe4e1;
            padding: 50px;
        }
        h1 {
            color: #d63384;
        }
        p {
            font-size: 20px;
        }
        .buttons {
            margin-top: 20px;
        }
        button {
            font-size: 18px;
            padding: 10px 20px;
            margin: 10px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
        }
        #yesBtn {
            background-color: #28a745;
            color: white;
        }
        #noBtn {
            background-color: #dc3545;
            color: white;
            position: absolute;
        }
    </style>
</head>
<body>
    <h1>I Love You! ❤</h1>
    <h2>Do you love me ? 💍</h2>
    <p>You are the best thing that ever happened to me!</p>

    <div class="buttons">
        <button id="yesBtn" onclick="alert('Yay! I knew you’d say YES! ❤')">Yes</button>
        <button id="noBtn" onmouseover="moveButton()">No</button>
    </div>

    <script>
        function moveButton() {
            let x = Math.random() * (window.innerWidth - 100);
            let y = Math.random() * (window.innerHeight - 50);
            document.getElementById('noBtn').style.left = ${x}px;
            document.getElementById('noBtn').style.top = ${y}px;
        }
    </script>
</body>
</html>
