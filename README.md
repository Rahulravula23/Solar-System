# Solar-System
<!DOCTYPE html>
<html lang="en">

<head>

    <title>Solar System</title>
    <style>
        body {
            margin: 0;
            height: 100vh;
            display: flex;
            background-color: black;
            align-items: center;
            justify-content: center;
            overflow: hidden;



        }

        .contanier {
            font-size: 10px;
            width: 40em;
            height: 40em;
            position: absolute;
            left: 300em;
            align-content: center;
            align-items: center;
            justify-content: center;
            display: flex;
        }

        .sun {
            height: 10em;
            width: 10em;
            top: 15em;
            left: 15em;

            background-color: orange;
            border-radius: 50%;

            position: absolute;
            box-shadow: 0 0 3em white;
        }

        .earth,
        .moon {
            position: absolute;
            border-style: solid;
            border-color: white transparent transparent transparent;
            border-width: 0.1em 0.1em 0 0;
            border-radius: 50%;


        }

        .earth {
            top: 5em;
            left: 5em;
            width: 30em;
            height: 30em;
            animation: orbit 38.7s linear infinite;
        }

        .moon {
            top: 0;
            right: 0;
            width: 8em;
            height: 8em;
            animation: orbit 2.7s linear infinite;
        }

        .earth::before,
        .moon::before {
            content: '';
            position: absolute;
            border-radius: 50%;
        }

        .earth::before {
            top: 2.8em;
            right: 2.8em;
            width: 3em;
            height: 3em;
            background-color: aquamarine;
        }

        .moon::before {
            top: 0.8em;
            right: 0.2em;
            width: 1.2em;
            height: 1.2em;
            background-color: silver;

        }

        @keyframes orbit {
            to {
                transform: rotate(360deg);
            }

        }
    </style>
</head>

<body>
    <div class="container">
        <div class="sun"></div>
        <div class="earth">
            <div class="moon"></div>

        </div>

    </div>

</body>

</html>
