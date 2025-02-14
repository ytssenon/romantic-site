html_code_fixed = """<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>For Chopa</title>
    <style>
        body {
            background-color: #ffe4e1;
            text-align: center;
            font-family: "Arial", sans-serif;
        }
        h1 {
            color: #ff69b4;
            font-size: 3em;
            font-family: "Brush Script MT", cursive;
        }
        .video-container {
            margin-top: 20px;
        }
        .video-container button {
            background-color: #ff69b4;
            color: white;
            font-size: 1.2em;
            padding: 10px 20px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
        .video-container button:hover {
            background-color: #ff1493;
        }
        .message {
            margin-top: 40px;
            font-size: 1.5em;
            font-style: italic;
            color: #d87093;
        }
        iframe {
            margin-top: 10px;
            border-radius: 10px;
            display: none; /* Скрываем видео по умолчанию */
        }
    </style>
    <script>
        function showVideo() {
            document.getElementById('videoFrame').style.display = 'block';
            document.getElementById('watchButton').style.display = 'none';
        }
    </script>
</head>
<body>

    <h1>For Chopa</h1>

    <div class="video-container">
        <p>А вот и наше первое видео ^-^</p>
        <button id="watchButton" onclick="showVideo()">Посмотреть</button>
        <iframe id="videoFrame" width="560" height="315" 
            src="https://www.youtube.com/embed/FOggJF2ipcU" 
            title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; 
            clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen>
        </iframe>
    </div>

    <div class="message">
        <p>Все что всегда я хотел с тобой – сделать тебя искренне счастливым человеком, понимая твои преграды и расстройства в жизни.</p>
    </div>

</body>
</html>
"""
