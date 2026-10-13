
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>دعوة زفاف - مصطفى & أماني</title>
    <!-- Google Fonts -->
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Amiri:wght@400;700&family=Reem+Kufi:wght@400;600;700&display=swap" rel="stylesheet">
    <style>
        :root {
            --gold: #d4af37;
            --gold-light: #f3e5ab;
            --dark-bg: #0d0d0d;
            --card-bg: #161616;
            --text-main: #f5f5f5;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
        }

        body {
            background-color: var(--dark-bg);
            color: var(--text-main);
            font-family: 'Amiri', serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            padding: 15px;
            background-image: radial-gradient(circle at center, #1f1f1f 0%, #080808 100%);
        }

        .invitation-container {
            background-color: var(--card-bg);
            border: 2px solid var(--gold);
            border-radius: 20px;
            padding: 35px 20px;
            max-width: 500px;
            width: 100%;
            text-align: center;
            box-shadow: 0 15px 35px rgba(212, 175, 55, 0.2);
            position: relative;
            outline: 1px solid var(--gold);
            outline-offset: -8px;
        }

        .bismillah {
            font-size: 1.3rem;
            color: var(--gold-light);
            margin-bottom: 15px;
        }

        .title {
            font-family: 'Reem Kufi', sans-serif;
            font-size: 2rem;
            color: var(--gold);
            margin-bottom: 15px;
            letter-spacing: 1px;
        }

        .families {
            font-size: 1rem;
            color: #d1d1d1;
            line-height: 1.8;
            margin-bottom: 20px;
        }

        .couple-names {
            font-family: 'Reem Kufi', sans-serif;
            font-size: 2.3rem;
            color: var(--gold-light);
            margin: 15px 0;
            text-shadow: 0 0 12px rgba(212, 175, 55, 0.4);
        }

        .details-box {
            border-top: 1px solid var(--gold);
            border-bottom: 1px solid var(--gold);
            padding: 18px 0;
            margin: 20px 0;
            line-height: 1.9;
            font-size: 1.1rem;
        }

        .highlight {
            color: var(--gold);
            font-weight: bold;
        }

        /* العداد التنازلي */
        .timer-container {
            display: flex;
            justify-content: center;
            gap: 10px;
            margin: 20px 0;
        }

        .timer-box {
            background: rgba(212, 175, 55, 0.08);
            border: 1px solid var(--gold);
            border-radius: 8px;
            padding: 8px;
            min-width: 65px;
        }

        .timer-number {
            font-size: 1.4rem;
            color: var(--gold-light);
            font-weight: bold;
        }

        .timer-label {
            font-size: 0.75rem;
            color: #bbb;
        }

        /* الأزرار */
        .btn-group {
            display: flex;
            flex-direction: column;
            gap: 10px;
            margin-top: 20px;
        }

        .btn {
            background-color: transparent;
            color: var(--gold);
            border: 1px solid var(--gold);
            padding: 11px 15px;
            border-radius: 25px;
            text-decoration: none;
            font-size: 0.95rem;
            font-weight: bold;
            transition: all 0.3s ease;
            cursor: pointer;
            font-family: 'Reem Kufi', sans-serif;
        }

        .btn:hover {
            background-color: var(--gold);
            color: #000;
            box-shadow: 0 0 12px rgba(212, 175, 55, 0.4);
        }

        .footer-note {
            margin-top: 15px;
            font-size: 0.85rem;
            color: #888;
        }
    </style>
</head>
<body>

    <div class="invitation-container">
        <div class="bismillah">بِسْمِ اللَّهِ الرَّحْمَٰنِ الرَّحِيمِ</div>
        <h1 class="title">دعوة زفاف مباركة</h1>
        
        <p class="families">
            بكل الحب والمودة، تتشرف<br>
            <b>آل مصطفى </b> و <b>عائلة
            آل فتيان</b><br>
            بدعوتكم لمشاركتهم فرحة العمر بمناسبة عقد قران أبنائهم:
        </p>

        <div class="couple-names">
            مصطفى & أماني
        </div>

        <div class="details-box">
            <p>🗓 <b>اليوم والتاريخ:</b> يوم الاثنين الموافق <span class="highlight">19-10-2026</span></p>
            <p>⏰ <b>الوقت:</b> من الساعة <span class="highlight">7:30 مساءً</span> ولغاية <span class="highlight">11:00 مساءً</span></p>
            <p>📍 <b>المكان:</b> فندق سراج - جبل الحسين</p>
            <p style="font-size: 0.9rem; color: #ccc;">(بجانب مستشفى الكندي)</p>
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

        <!-- الأزرار التفاعلية -->
        <div class="btn-group">
            <a href="https://maps.google.com/?q=Siraj+Hotel+Amman+Al_Hussein+Hospital" target="_blank" class="btn">📍 موقع الفندق على الخريطة</a>
            <button onclick="addToCalendar()" class="btn">📅 إضافة الموعد إلى التقويم</button>
        </div>

        <p class="footer-note">حضوركم يسعدنا ويزيد ليلتنا بهجة وسروراً</p>
    </div>

    <script>
        // إعداد التاريخ المستهدف للزفاف
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
                document.querySelector(".timer-container").innerHTML = "<p style='color:var(--gold); font-weight:bold; font-size:1.1rem;'>أهلاً وسهلاً بكم في حفل زفافنا اليوم!</p>";
            }
        };

        setInterval(updateCountdown, 1000);
        updateCountdown();

        // دالة إضافة الموعد لتقويم جوجل
        function addToCalendar() {
            const title = encodeURIComponent("حفل زفاف مصطفى وأماني");
            const details = encodeURIComponent("حفل زفاف مصطفى وأماني في فندق سراج - جبل الحسين، بجانب مستشفى الكندي.");
            const location = encodeURIComponent("فندق سراج، جبل الحسين، عمان، الأردن");
            const calendarUrl = `https://calendar.google.com/calendar/render?action=TEMPLATE&text=${title}&dates=20261019T163000Z/20261019T200000Z&details=${details}&location=${location}`;
            window.open(calendarUrl, '_blank');
        }
    </script>
</body>
</html>
