<!DOCTYPE html>
<html lang="th">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Student Profile | จรินทร์พรรณ แก้วเคียงคำ</title>
    
    <link href="https://fonts.googleapis.com/css2?family=Kanit:wght@300;400;600&family=Mali:wght@400;600&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        :root {
            --primary-pink: #ff85a1;
            --primary-red: #e63946;
            --soft-pink: #ffe5ec;
            --text-dark: #2b2d42;
            --bg-gradient: linear-gradient(135deg, #ff9a9e 0%, #fecfef 100%);
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Kanit', sans-serif;
        }

        body {
            background: var(--bg-gradient);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 40px 20px;
            overflow-x: hidden;
            position: relative;
        }

        /* Animation Elements */
        .decoration {
            position: fixed;
            pointer-events: none;
            z-index: 0;
            filter: drop-shadow(0 0 5px rgba(255,255,255,0.8));
        }

        @keyframes float {
            0% { transform: translate(0, 0) rotate(0deg); }
            50% { transform: translate(20px, -20px) rotate(10deg); }
            100% { transform: translate(0, 0) rotate(0deg); }
        }

        @keyframes sparkle {
            0%, 100% { opacity: 0.3; transform: scale(1); }
            50% { opacity: 1; transform: scale(1.2); }
        }

        /* Profile Card */
        .profile-card {
            background: rgba(255, 255, 255, 0.95);
            width: 100%;
            max-width: 800px;
            border-radius: 30px;
            box-shadow: 0 20px 50px rgba(230, 57, 70, 0.15);
            overflow: hidden;
            position: relative;
            z-index: 1;
            border: 8px solid white;
            display: flex;
            flex-wrap: wrap;
        }

        /* Left Side: Header & Basic Info */
        .sidebar {
            flex: 1;
            min-width: 300px;
            background: #fff0f3;
            padding: 40px 30px;
            text-align: center;
            border-right: 1px dashed var(--primary-pink);
        }

        .profile-img-container {
            width: 180px;
            height: 180px;
            margin: 0 auto 20px;
            background: white;
            border-radius: 50%;
            border: 5px solid var(--primary-pink);
            display: flex;
            justify-content: center;
            align-items: center;
            position: relative;
        }

        .profile-img-container i {
            font-size: 80px;
            color: var(--primary-red);
        }

        .profile-img-container::after {
            content: '🐰';
            position: absolute;
            bottom: 5px;
            right: 5px;
            font-size: 40px;
        }

        .name-title {
            font-size: 1.5rem;
            color: var(--primary-red);
            font-weight: 600;
        }

        .school-info {
            font-size: 1.1rem;
            color: #666;
            margin-bottom: 20px;
        }

        .motto-box {
            background: var(--primary-red);
            color: white;
            padding: 15px;
            border-radius: 15px;
            font-size: 0.9rem;
            margin-top: 20px;
            font-family: 'Mali', cursive;
            position: relative;
        }

        /* Right Side: Details */
        .main-content {
            flex: 1.5;
            min-width: 350px;
            padding: 40px;
        }

        .section-title {
            font-size: 1.2rem;
            color: var(--primary-red);
            border-bottom: 2px solid var(--soft-pink);
            padding-bottom: 5px;
            margin-bottom: 15px;
            margin-top: 25px;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .grid-info {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 10px;
        }

        .info-item {
            font-size: 0.95rem;
            margin-bottom: 8px;
        }

        .info-label { font-weight: 600; color: #555; }

        /* Pills/Tags */
        .tag-container {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
            margin-top: 5px;
        }

        .tag {
            background: var(--soft-pink);
            color: var(--primary-red);
            padding: 4px 12px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
            border: 1px solid #ffb3c1;
        }

        .skill-tag { background: #e0f2f1; color: #00796b; border-color: #b2dfdb; }

        /* Printing A4 Support */
        @media print {
            body { background: white; padding: 0; }
            .profile-card { box-shadow: none; border: 1px solid #eee; }
            .decoration { display: none; }
        }

        /* Floating Items */
        .bunny { font-size: 30px; animation: float 6s infinite ease-in-out; }
        .sakura { color: #ffb7c5; font-size: 20px; animation: float 8s infinite linear; }
        .sparkle { color: gold; font-size: 15px; animation: sparkle 2s infinite; }

    </style>
</head>
<body>

    <img src="image_0.png" alt="ตัวละครอนิเมะ" style="height: 250px; width: 400px; object-fit: cover;">

    <div class="profile-card">
        <div class="sidebar">
            <div class="profile-img-container">
                <i class="fa-solid fa-user-graduate"></i>
            </div>
            <h1 class="name-title">ด.ญ.จรินทร์พรรณ แก้วเคียงคำ</h1>
            <p class="school-info">ชื่อเล่น: <b>สตางค์</b> | ชั้น ม.3/2</p>
            <p style="color: #888;"><i class="fa-solid fa-school"></i> โรงเรียนจอมทอง</p>

            <div class="motto-box">
                <i class="fa-solid fa-quote-left" style="opacity: 0.5;"></i><br>
                "ความพยายามอยู่ที่ไหน ความสำเร็จอยู่ที่นั่น"<br>
                <i class="fa-solid fa-quote-right" style="opacity: 0.5; float: right;"></i>
            </div>

            <div class="section-title"><i class="fa-solid fa-address-card"></i> ข้อมูลทั่วไป</div>
            <div style="text-align: left; font-size: 0.9rem;">
                <p><b>เพศ:</b> หญิง | <b>กรุ๊ปเลือด:</b> O</p>
                <p><b>วันเกิด:</b> 17 ตุลาคม 2554</p>
                <p><b>ราศี:</b> ตุลย์ | <b>ส่วนสูง:</b> 162 ซ.ม.</p>
                <p><b>ภูมิลำเนา:</b> เชียงใหม่</p>
            </div>
        </div>

        <div class="main-content">
            
            <div class="section-title"><i class="fa-solid fa-book-open"></i> การเรียน & ความฝัน</div>
            <div class="grid-info">
                <div class="info-item"><span class="info-label">วิชาที่ชอบ:</span> <span style="color: green;">วิทยาศาสตร์</span></div>
                <div class="info-item"><span class="info-label">วิชาที่ยาก:</span> <span style="color: red;">วิทยาศาสตร์</span></div>
                <div class="info-item"><span class="info-label">อาชีพในฝัน:</span> <b>พยาบาล 🏥</b></div>
                <div class="info-item"><span class="info-label">ชมรม:</span> Karaoke 🎤</div>
            </div>

            <div class="section-title"><i class="fa-solid fa-heart"></i> สิ่งที่ชอบ</div>
            <div class="info-item"><span class="info-label">อาหารโปรด:</span> ข้าวคลุกกะปิ</div>
            <div class="info-item"><span class="info-label">สีที่ชอบ:</span> <span class="tag" style="background: red; color: white;">แดง</span></div>
            <div class="info-item"><span class="info-label">เพลง:</span> เพลงของยังโอม (Youngohm)</div>
            <div class="info-item"><span class="info-label">อนิเมะ:</span> เซอร์แวมพ์ (Servamp)</div>

            <div class="section-title"><i class="fa-solid fa-star"></i> ทักษะ & งานอดิเรก</div>
            <div class="tag-container">
                <span class="tag skill-tag">🎨 วาดรูป</span>
                <span class="tag skill-tag">🎤 ร้องเพลง</span>
                <span class="tag">🎬 ดูอนิเมะ</span>
                <span class="tag">🥎 เปตอง</span>
            </div>

            <div class="section-title"><i class="fa-solid fa-users"></i> เพื่อนสนิท</div>
            <div class="tag-container">
                <span class="tag" style="background: white;">ปั้นหยา</span>
                <span class="tag" style="background: white;">อิ่มเอม</span>
                <span class="tag" style="background: white;">แก้มหอม</span>
                <span class="tag" style="background: white;">เมกาน</span>
            </div>

            <div class="section-title"><i class="fa-solid fa-image"></i> รูปภาพของฉัน</div>
            <div style="text-align: center; margin-top: 15px;">
                <img src="ใส่ลิงก์รูปภาพตรงนี้.jpg" alt="Student Photo" style="width: 400px; height: 250px; object-fit: cover; border-radius: 15px; border: 4px solid var(--soft-pink); box-shadow: 0 5px 15px rgba(0,0,0,0.05);">
            </div>

        </div>
    </div>

</body>
</html>
