<!DOCTYPE html>
<html>
<head>
    <title>Colour Trading Game</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            text-align: center;
            background-color: #f4f4f4;
        }
        h1 {
            color: #333;
        }
        .color-box {
            width: 200px;
            height: 200px;
            margin: 20px auto;
            border-radius: 10px;
        }
        button {
            padding: 10px 20px;
            margin: 10px;
            font-size: 18px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <h1>Colour Trading Game</h1>
    <div id="colorBox" class="color-box"></div>
    <p id="resultText"></p>
    <button onclick="chooseColor('Red')">Red</button>
    <button onclick="chooseColor('Green')">Green</button>

    <script>
        const colors = ['Red', 'Green'];
        let currentColor = '';

        function generateColor() {
