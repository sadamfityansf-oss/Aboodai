# Aboodai
Wedding card
<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>دعوة زفاف مصطفى وأماني</title>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Amiri:ital,wght@0,400;0,700;1,400&family=Reem+Kufi:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --primary-gold: #d4af37;
            --accent-gold: #f3e5ab;
            --bg-black: #121212;
            --card-black: #1e1e1e;
            --text-gold: #e6ca65;
            --text-light: #f5f5f5;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            background-color: var(--bg-black);
            color: var(--text-light);
            font-family: 'Amiri', serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 20px;
            background-image: radial-gradient(circle at center, #222222 0%, #0a0a0a 100%);
        }

        .invitation-card {
            background-color: var(--card-black);
            border: 2px solid var(--primary-gold);
            border-radius: 16px;
            padding: 40px 25px;
            max-width: 550px;
            width: 100%;
            text-align: center;
            box-shadow: 0 10px 30px rgba(212, 175, 55, 0.15);
            position: relative;
            outline: 1px solid var(--primary-gold);
            outline-offset: -10px;
        }

        .header-title {
            font-family: 'Reem Kufi', sans-serif;
            font-size: 2.2rem;
            color: var(--primary-gold);
            margin-bottom: 10px;
            letter-spacing: 1px;
        }

        .family-names {
            font-size: 1.1rem;
            color: #ccc;
            margin-bottom: 25px;
            line-height: 1.8;
        }

        .couple-names {
            font-family: 'Reem Kufi', sans-serif;
            font-size: 2.6rem;
            color: var(--accent-gold);
            margin: 20px 0;
            text-shadow: 0 0 10px rgba(212, 175, 55, 0.3);
        }

        .details-box {
            border-top: 1px solid var(--primary-gold);
            border-bottom: 1px solid var(--primary-gold);
            padding: 20px 0;
            margin: 25px 0;
            line-height: 2;
            font-size: 1.2rem;
        }

        .highlight {
            color: var(--primary-gold);
            font-weight: bold;
        }

        /* Countdown Timer */
        .timer-container {
            display: flex;
            justify-content: center;
            gap: 15px;
            margin: 25px 0;
        }

        .timer-box {
            background: rgba(212, 175, 55, 0.1);
            border: 1px solid var(--primary-gold);
            border-radius: 8px;
            padding: 10px;
            min-width: 70px;
        }

        .timer-number {
            font-size: 1.5rem;
            color: var(--accent-gold);
            font-weight: bold;
        }

        .timer-label {
            font-size: 0.8rem;
            color: #aaa;
        }

        /* Action Buttons */
        .btn-group {
            display: flex;
            flex-direction: column;
            gap: 12px;
            margin-top: 25px;
        }

        .btn {
            background-color: transparent;
            color: var(--primary-gold);
            border: 1px solid var(--primary-gold);
            padding: 12px 20px;
            border-radius: 25px;
            text-decoration: none;
            font-size: 1rem;
            font-weight: bold;
            transition: all 0.3s ease;
            cursor: pointer;
        }

        .btn:hover {
            background-color: var(--primary-gold);
            color: #000;
            box-shadow: 0 0 15px rgba(212, 175, 55, 0.4);
        }

        @media (max-width: 480px) {
            .header-title { font-size: 1.8rem; }
            .couple-names { font-size: 2.1rem; }
            .details-box { font-size: 1.05rem; }
            .timer-box { min-width: 55px; }
        }
    </style>
</head>
<body>

    <div class="invitation-card">
        <h1 class="header-title">دعوة زفاف</h1>
        
        <p class="family-names">
            يتشرف **عائلة مصطفى** و **عائلة فتيان**<br>
            بدعوتكم لمشاركتهم فرحة العمر بمناسبة عقد قران أبنائهم
        </p>

        <div class="couple-names">
            مصطفى <span style="font-size: 1.8rem; color: var(--primary-gold);">&</span> أماني
        </div>

        <div class="details-box">
            <p>🗓 <b>اليوم:</b> يوم الاثنين - الموافق <span class="highlight">19-10-2026</span></p>
            <p>⏰ <b>الوقت:</b> من الساعة <span class="highlight">7:30 مساءً</span> ولغاية <span class="highlight">11:00 مساءً</span></p>
            <p>📍 <b>المكان:</b> فندق سراج - جبل الحسين</p>
            <p style="font-size: 0.95rem; color: #aaa;">(بجانب مستشفى الكندي)</p>
        </div>

        <!-- العداد التنازلي -->
        <div class="timer-container">
            <div class="timer-box">
                <div id="days" class="timer-number">00</div>
                <div class="timer-label">يوم</div>
            </div>
            <div class="timer-box">
                <div id="hours" class="timer-number">00</div>
                <div class="timer-label">ساعة</div>
            </div>
            <div class="timer-box">
                <div id="minutes" class="timer-number">00</div>
                <div class="timer-label">دقيقة</div>
            </div>
            <div class="timer-box">
                <div id="seconds" class="timer-number">00</div>
                <div class="timer-label">ثانية</div>
            </div>
        </div>

        <!-- أزرار التفاعل -->
        <div class="btn-group">
            <a href="https://maps.google.com/?q=Siraj+Hotel+Amman" target="_blank" class="btn">📍 موقع الفندق على الخريطة</a>
            <button onclick="addToCalendar()" class="btn">📅 إضافة إلى التقويم</button>
        </div>
    </div>

    <script>
        // إعداد تاريخ المناسبة
        const targetDate = new Date("October 19, 2026 19:30:00").getTime();

        const updateCountdown = () => {
            const now = new Date().getTime();
            const difference = targetDate - now;

            if (difference > 0) {
                const days = Math.floor(difference / (1000 * 60 * 60 * 24));
                const hours = Math.floor((difference % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60));
                const minutes = Math.floor((difference % (1000 * 60 * 60)) / (1000 * 60));
                const seconds = Math.floor((difference % (1000 * 60)) / 1000);

                document.getElementById("days").innerText = days.toString().padStart(2, '0');
                document.getElementById("hours").innerText = hours.toString().padStart(2, '0');
                document.getElementById("minutes").innerText = minutes.toString().padStart(2, '0');
                document.getElementById("seconds").innerText = seconds.toString().padStart(2, '0');
            } else {
                document.querySelector(".timer-container").innerHTML = "<p style='color:var(--primary-gold); font-weight:bold;'>أهلاً وسهلاً بكم في حفلنا!</p>";
            }
        };

        setInterval(updateCountdown, 1000);
        updateCountdown();

        // إضافة الحدث لتقويم جوجل
        function addToCalendar() {
            const title = encodeURIComponent("حفل زفاف مصطفى وأماني");
            const details = encodeURIComponent("حفل زفاف مصطفى وأماني في فندق سراج - جبل الحسين بجانب مستشفى الكندي.");
            const location = encodeURIComponent("فندق سراج، جبل الحسين، عمان");
            const calendarUrl = `https://calendar.google.com/calendar/render?action=TEMPLATE&text=${title}&dates=20261019T163000Z/20261019T200000Z&details=${details}&location=${location}`;
            window.open(calendarUrl, '_blank');
        }
    </script>
</body>
</html>
