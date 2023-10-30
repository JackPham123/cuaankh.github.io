<!DOCTYPE html>
<html>
<head>
    <style>
        .heart {
            position: relative;
            width: 100px;
            height: 90px;
            background-color: red;
            animation: heartbeat 1s infinite;
        }

        .heart::before,
        .heart::after {
            content: '';
            position: absolute;
            top: 0;
            width: 100px;
            height: 100px;
            border-radius: 100px 100px 0 0;
            background-color: red;
        }

        .heart::before {
            left: -50px;
        }

        .heart::after {
            left: 50px;
        }

        @keyframes heartbeat {
            0%, 100% {
                transform: scale(1);
            }
            50% {
                transform: scale(1.1);
            }
        }
    </style>
</head>
<body>
    <div class="heart"></div>
</body>
</html>
