<!DOCTYPE html>
<html lang="fa">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>وب‌سایت اشعار</title>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Nastaliq+Urdu&family=Vazir:wght@400;700&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Noto Nastaliq Urdu', serif;
            background: linear-gradient(to right, #FFDEE9, #B5FFFC);
            color: #333;
            margin: 0;
            padding: 0;
            overflow-x: hidden;
            direction: rtl;
        }

        header {
            background-color: #333;
            color: #FFF;
            padding: 5px 0;
            text-align: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .title-small, .meaning-text, .verse-meaning {
            font-family: 'Vazir', sans-serif;
            font-size: 1em;
        }

        .title-large {
            font-family: 'Vazir', sans-serif;
            font-size: 1.5em;
        }

        nav {
            display: flex;
            justify-content: center;
            background-color: #444;
            position: sticky;
            top: 50px;
            z-index: 998;
            padding: 5px 0;
        }

        nav a {
            color: #FFF;
            padding: 10px 15px;
            text-decoration: none;
            font-family: 'Vazir', sans-serif;
            font-size: 0.8em;
        }

        .content {
            padding: 20px;
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        .section {
            margin: 20px 0;
            padding: 20px;
            border: 1px solid #DDD;
            background-color: #FFF;
            box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
            width: 80%;
            max-width: 800px;
        }

        h2 {
            font-family: 'Vazir', sans-serif;
            font-weight: 700;
            text-align: center;
            background-color: #333;
            color: #FFF;
            padding: 10px;
        }

        h3 {
            font-family: 'Vazir', sans-serif;
            font-weight: 700;
            text-align: center;
            background-color: #f0f0f0;
            color: #333;
            padding: 5px;
        }

        .poet-name {
            font-family: 'Noto Nastaliq Urdu', serif;
            text-align: center;
            font-size: 1.2em;
            font-weight: bold;
            color: #444;
        }

        .search-container {
            position: absolute;
            left: 10px;
            top: 10px;
            display: flex;
            align-items: center;
        }

        .search-box {
            width: 200px;
            padding: 5px;
            font-family: 'Vazir', sans-serif;
        }

        .search-button {
            padding: 5px 10px;
            background-color: #444;
            color: white;
            border: none;
            cursor: pointer;
            font-family: 'Vazir', sans-serif;
        }
    </style>
    <script>
        function searchContent() {
            var input = document.getElementById("search").value.toLowerCase();
            var sections = document.querySelectorAll(".section");
            sections.forEach(function(section) {
                if (section.innerText.toLowerCase().includes(input)) {
                    section.style.display = "block";
                } else {
                    section.style.display = "none";
                }
            });
        }
    </script>
</head>
<body>
    <header>
        <h1 class="title-small">بسم الله الرحمن الرحیم</h1>
        <h1 class="title-large">وب‌سایت اشعار</h1>
        <div class="search-container">
            <input id="search" class="search-box" type="text" placeholder="جستجو کنید...">
            <button class="search-button" onclick="searchContent()">جستجو کردن</button>
        </div>
    </header>
    <nav>
        <a href="#poems">اشعار</a>
        <a href="#quotes">جملات ناب</a>
        <a href="#articles">مقاله‌ها</a>
        <a href="#meaningful-content">مطالب پر معنا</a>
        <a href="#quran-verses">آیات زیبا قرآنکریم</a>
    </nav>
    <div class="content">
        <div class="section" id="poems">
            <h2>اشعار</h2>
            <p>بنی‌آدم اعضای یکدیگرند<br>که در آفرینش ز یک گوهرند</p>
            <p class="poet-name">سعدی شیرازی</p>
            <h3>معنای شعر</h3>
            <p class="meaning-text">تمام انسان‌ها اعضای یک پیکرند و از یک گوهر آفریده شده‌اند، پس باید با یکدیگر مهربان باشند.</p>
        </div>
        <div class="section" id="quotes">
            <h2>جملات ناب</h2>
            <p>«آنکه در طلب کمال است، همواره در حال شدن است.»</p>
            <p class="poet-name">مولانا</p>
        </div>
        <div class="section" id="articles">
            <h2>مقاله‌ها</h2>
            <p class="meaning-text">علم یکی از بزرگ‌ترین سرمایه‌های بشریت است ...</p>
        </div>
        <div class="section" id="meaningful-content">
            <h2>مطالب پر معنا</h2>
            <p>دوستی واقعی، نه در کلام، بلکه در رفتار نمایان می‌شود.</p>
        </div>
        <div class="section" id="quran-verses">
            <h2>آیات زیبا قرآنکریم</h2>
            <p>وَإِن يَكَادُ الَّذِينَ كَفَرُوا لَيُزْلِقُونَكَ بِأَبْصَارِهِمْ ...</p>
            <h3>معنای آیه</h3>
            <p class="verse-meaning">و کسانی که کفر ورزیدند، وقتی ذکر (قرآن) را شنیدند ...</p>
        </div>
    </div>
</body>
</html# -
این سایت توسط احمدشجاع نجات طراحی شده است
