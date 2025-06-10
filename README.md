
<html lang="th">
<head>
    <link rel="manifest" href="manifest.json">
    <meta name="theme-color" content="#8d6e63"> 
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ยินดีต้อนรับสู่ ชาววังเย็น คาเฟ่</title> <link href="https://fonts.googleapis.com/css2?family=Kanit:wght@300;400;500;600&family=Pridi:wght@300;400&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        :root {
            --bg-color: #fdfaf6;
            --primary-color: #8d6e63;
            --text-color: #4e342e;
            --button-bg: var(--primary-color);
            --button-text: #ffffff;
            --button-hover-bg: #6d4c41;
            --font-heading: 'Pridi', serif;
            --font-body: 'Kanit', sans-serif;
        }
        html, body {
            height: 100%;
            margin: 0;
        }
        body {
            font-family: var(--font-body);
            background-color: var(--bg-color);
            color: var(--text-color);
            display: flex;
            justify-content: center;
            align-items: center;
            text-align: center;
            padding: 20px;
             background: linear-gradient(rgba(253, 250, 246, 0.8), rgba(253, 250, 246, 0.8)), url('https://placehold.co/1920x1080/a1887f/fdfaf6?text=Cafe+Background') no-repeat center center fixed; /* <<< ใส่ URL รูปพื้นหลังร้าน */
            background-size: cover;
        }
        .landing-content {
            max-width: 600px;
            background-color: rgba(255, 255, 255, 0.9); /* เพิ่มพื้นหลังให้ข้อความอ่านง่าย */
            padding: 40px;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        }
        .logo-image {
            max-width: 150px;
            margin-bottom: 20px;
        }
        h1 {
            font-family: var(--font-heading);
            color: var(--primary-color);
            font-size: clamp(2rem, 6vw, 3rem); /* ปรับขนาดตามหน้าจอ */
            margin-bottom: 15px;
        }
        p {
            font-size: clamp(1rem, 3vw, 1.2rem);
            color: var(--text-light-color, #795548);
            margin-bottom: 30px;
        }
        .btn {
            display: inline-block;
            background-color: var(--button-bg);
            color: var(--button-text);
            padding: 12px 30px;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: clamp(1rem, 3vw, 1.1rem);
            font-weight: 500;
            text-decoration: none;
            transition: background-color 0.2s ease, transform 0.1s ease;
        }
        .btn:hover {
            background-color: var(--button-hover-bg);
            transform: translateY(-2px);
        }
         .btn i { margin-right: 8px; }
    </style>
</head>

    <div class="landing-content">
        <h1>ชาววังเย็น คาเฟ่</h1> <p>สัมผัสรสชาติกาแฟแท้และเบเกอรี่โฮมเมด</p>
        <a href="shop.html" class="btn"><i class="fas fa-store"></i> ดูเมนูและสั่งซื้อ</a>
    </div>
    <script>
        if ('serviceWorker' in navigator) {
            window.addEventListener('load', () => {
                navigator.serviceWorker.register('./sw.js') // ต้องแน่ใจว่า path ถูกต้อง
                    .then(registration => {
                        console.log('ServiceWorker registration successful with scope: ', registration.scope);
                    })
                    .catch(error => {
                        console.log('ServiceWorker registration failed: ', error);
                    });
            });
        }
    </script>
