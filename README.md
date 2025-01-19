<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
            background-color: #f5f5f5;
            font-family: 'Arial', sans-serif;
        }
        .valentine {
            text-align: center;
            font-size: 2rem;
            color: #e91e63;
        }
        .heart {
            width: 100px;
            height: 90px;
            position: relative;
            margin: 20px auto;
            animation: beat 1s infinite;
        }
        .heart::before,
        .heart::after {
            content: '';
            width: 100px;
            height: 150px;
            background: #e91e63;
            position: absolute;
            border-radius: 100px 100px 0 0;
            transform: rotate(-45deg);
            transform-origin: 0 100%;
        }
        .heart::after {
            left: 100px;
            transform: rotate(45deg);
            transform-origin: 100% 100%;
        }
        @keyframes beat {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.1);
            }
        }
    </style>
    <title>Valentine Letter</title>
</head>
<body>
    <div class="valentine">
        <div class="heart"></div>
        <p>Hi loveeeeeeeeeeeeeeyyyyy Marie, will you be my valentine this coming feb 14? mwehehehe ❤️</p>
    </div>
</body>
</html>
