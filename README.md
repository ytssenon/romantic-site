html_code_youtube = """<!DOCTYPE html>
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
        .message {
            margin-top: 40px;
            font-size: 1.5em;
            font-style: italic;
            color: #d87093;
        }
        iframe {
            margin-top: 10px;
            border-radius: 10px;
        }
    </style>
</head>
<body>

    <h1>For Chopa</h1>

    <div class="video-container">
        <p>А вот и наше первое видео ^-^</p>
        <iframe width="560" height="315" src="https://www.youtube.com/embed/FOggJF2ipcU" 
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

# Сохраняем обновленный HTML-файл
file_path_youtube = "/mnt/data/index.html"
with open(file_path_youtube, "w", encoding="utf-8") as file:
    file.write(html_code_youtube)

# Создаём ZIP-архив с новым HTML-файлом
zip_path_youtube = "/mnt/data/romantic_site.zip"
with zipfile.ZipFile(zip_path_youtube, 'w') as zipf:
    zipf.write(file_path_youtube, arcname="index.html")

# Предоставляем ссылку на скачивание
zip_path_youtube
