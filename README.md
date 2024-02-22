<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f4f4f4;
            display: flex;
            justify-content: center;
            align-items: center;
            height: 100vh;
        }

        #post-it-container {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }

        .post-it {
            width: 200px;
            height: 150px;
            padding: 10px;
            border-radius: 5px;
            box-shadow: 2px 2px 5px rgba(0, 0, 0, 0.2);
            position: relative;
        }

        .post-it:before {
            content: "";
            position: absolute;
            top: 0;
            left: 50%;
            width: 0;
            height: 0;
            border-style: solid;
            border-width: 0 15px 15px 15px;
            border-color: transparent transparent transparent transparent;
            transform: translateX(-50%);
        }

        .post-it-content {
            height: 100%;
        }

        /* Color variations */
        .post-it.red {
            background-color: #ff8a80;
        }

        .post-it.light-blue {
            background-color: #80d8ff;
        }

        .post-it.green {
            background-color: #a5d6a7;
        }

        .post-it.orange {
            background-color: #ffcc80;
        }

        .post-it.yellow {
            background-color: #ffff8d;
        }
    </style>
    <title>Post-It Notes Page</title>
</head>
<body>

    <div id="post-it-container">
        <div class="post-it red">
            <div class="post-it-content">
                <p>Note 1</p>
            </div>
        </div>

        <div class="post-it light-blue">
            <div class="post-it-content">
                <p>Note 2</p>
            </div>
        </div>

        <div class="post-it green">
            <div class="post-it-content">
                <p>Note 3</p>
            </div>
        </div>

        <div class="post-it orange">
            <div class="post-it-content">
                <p>Note 4</p>
            </div>
        </div>

        <div class="post-it yellow">
            <div class="post-it-content">
                <p>Note 5</p>
            </div>
        </div>
    </div>

</body>
</html>
