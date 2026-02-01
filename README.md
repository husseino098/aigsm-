<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>تطبيق اتصال فيديو بسيط</title>
    <style>
        body { font-family: sans-serif; text-align: center; background: #f0f2f5; }
        .video-container { display: flex; justify-content: center; gap: 10px; flex-wrap: wrap; margin-top: 20px; }
        video { width: 300px; background: #000; border-radius: 10px; box-shadow: 0 4px 8px rgba(0,0,0,0.2); }
        .controls { margin-top: 20px; }
        button { padding: 10px 20px; font-size: 16px; cursor: pointer; border-radius: 5px; border: none; background: #007bff; color: white; }
        button:hover { background: #0056b3; }
    </style>
</head>
<body>

    <h2>اتصال فيديو عبر المتصفح</h2>

    <div class="video-container">
        <div>
            <p>فيديو هاتفك (أنت)</p>
            <video id="localVideo" autoplay playsinline muted></video>
        </div>
        <div>
            <p>فيديو الطرف الآخر</p>
            <video id="remoteVideo" autoplay playsinline></video>
        </div>
    </div>

    <div class="controls">
        <button id="startButton">تشغيل الكاميرا</button>
        <button id="callButton">بدء الاتصال</button>
    </div>

    <script src="script.js"></script>
</body>
</html>
