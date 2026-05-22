<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Profile | จรินทร์พรรณ แก้วเคียงคำ</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Kanit:wght@300;400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        :root {
            --primary-color: #e63946; 
            --secondary-color: #f1faee;
            --text-dark: #1d3557;
            --bg-gradient: linear-gradient(135deg, #ff4d4d 0%, #a70000 100%);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Kanit', sans-serif;
        }

        body {
            background-color: #f8f9fa;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
        }

        .profile-card {
            background: white;
            width: 100%;
            max-width: 450px;
            border-radius: 20px;
            overflow: hidden;
            box-shadow: 0 15px 35px rgba(0,0,0,0.1);
            transition: transform 0.3s ease;
        }

        .profile-card:hover {
            transform: translateY(-10px);
        }

        .header-bg {
            background: var(--bg-gradient);
            height: 120px;
            position: relative;
        }

        .profile-img {
            width: 130px;
            height: 130px;
            background: #fff;
            border-radius: 50%;
            position: absolute;
            bottom: -65px;
            left: 50%;
            transform: translateX(-50%);
            display: flex;
            justify-content: center;
            align-items: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            border: 5px solid white;
        }

        .profile-img i {
            font-size: 60px;
            color: var(--primary-color);
        }

        .content {
            padding: 80px 30px 40px;
            text-align: center;
        }

        .name {
            font-size: 1.6rem;
            color: var(--text-dark);
            margin-bottom: 5px;
            font-weight: 600;
        }

        .nickname {
            font-size: 1.1rem;
            color: var(--primary-color);
            margin-bottom: 25px;
            font-weight: 400;
        }

        .info-list {
            text-align: left;
            margin-top: 20px;
        }

        .info-item {
            display: flex;
            align-items: center;
            margin-bottom: 15px;
            padding: 12px;
            background: #fff5f5;
            border-radius: 12px;
            border-left: 5px solid var(--primary-color);
        }

        .info-item i {
            width: 35px;
            font-size: 1.2rem;
            color: var(--primary-color);
        }

        .info-label {
            font-weight: 600;
            color: var(--text-dark);
            margin-right: 10px;
            min-width: 90px;
        }

        .info-value {
            color: #555;
        }

        .footer-tag {
            margin-top: 25px;
            font-size: 0.9rem;
            color: #bbb;
        }
    </style>
</head>
<body>

    <div class="profile-card">
        <div class="header-bg">
            <div class="profile-img">
                <i class="fa-solid fa-user-tie"></i>
            </div>
        </div>

        <div class="content">
            <h1 class="name">ด.ญ.จรินทร์พรรณ แก้วเคียงคำ</h1>
            <p class="nickname">ชื่อเล่น: <strong>น้องสตางค์</strong></p>

            <div class="info-list">
                <div class="info-item">
                    <i class="fa-solid fa-cake-candles"></i>
                    <span class="info-label">วันเกิด:</span>
                    <span class="info-value">17 ตุลาคม 2554</span>
                </div>

                <div class="info-item">
                    <i class="fa-solid fa-utensils"></i>
                    <span class="info-label">ของโปรด:</span>
                    <span class="info-value">ข้าวซอย</span>
                </div>

                <div class="info-item">
                    <i class="fa-solid fa-palette"></i>
                    <span class="info-label">สีที่ชอบ:</span>
                    <span class="info-value" style="color: #d90429; font-weight: bold;">สีแดง</span>
                </div>

                <div class="info-item">
                    <i class="fa-solid fa-flask"></i>
                    <span class="info-label">วิชาที่ชอบ:</span>
                    <span class="info-value">วิทยาศาสตร์</span>
                </div>
            </div>

            <p class="footer-tag">Nice to meet you! ✨</p>
        </div>
    </div>

</body>
</html>
