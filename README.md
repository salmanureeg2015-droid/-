<!DOCTYPE html>
<html lang="ar" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ريفل تاون | Rifle Town</title>

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: Tahoma, Arial, sans-serif;
        }

        body {
            background:
                radial-gradient(circle at top, #202630 0%, #090b0f 45%, #050608 100%);
            color: white;
            min-height: 100vh;
        }

        /* NAVBAR */

        nav {
            position: sticky;
            top: 0;
            z-index: 100;
            height: 75px;
            background: rgba(7, 9, 13, 0.94);
            border-bottom: 1px solid #292e37;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 0 7%;
            backdrop-filter: blur(15px);
        }

        .logo {
            font-size: 24px;
            font-weight: bold;
            letter-spacing: 2px;
        }

        .logo span {
            color: #9ca3af;
        }

        nav ul {
            list-style: none;
            display: flex;
            gap: 30px;
        }

        nav a {
            color: #d5d9df;
            text-decoration: none;
            transition: .3s;
        }

        nav a:hover {
            color: white;
        }

        /* HERO */

        .hero {
            min-height: 650px;
            display: flex;
            align-items: center;
            justify-content: center;
            text-align: center;
            padding: 60px 20px;
        }

        .hero-content {
            max-width: 900px;
        }

        .hero small {
            color: #aeb5bf;
            letter-spacing: 5px;
            font-size: 14px;
        }

        .hero h1 {
            font-size: clamp(55px, 9vw, 110px);
            margin: 20px 0 5px;
            letter-spacing: 7px;
        }

        .hero h2 {
            font-size: 22px;
            color: #9da5b1;
            letter-spacing: 8px;
            margin-bottom: 25px;
        }

        .hero p {
            color: #aeb5bf;
            font-size: 18px;
            line-height: 2;
            margin-bottom: 35px;
        }

        .buttons {
            display: flex;
            justify-content: center;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            padding: 15px 35px;
            border-radius: 7px;
            text-decoration: none;
            color: #080a0e;
            background: white;
            font-weight: bold;
            transition: .3s;
        }

        .btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 10px 30px rgba(255,255,255,.12);
        }

        .btn.dark {
            background: #171b22;
            color: white;
            border: 1px solid #303641;
        }

        /* SECTIONS */

        section {
            max-width: 1150px;
            margin: auto;
            padding: 90px 25px;
        }

        .title {
            text-align: center;
            margin-bottom: 45px;
        }

        .title h2 {
            font-size: 35px;
            margin-bottom: 10px;
        }

        .title p {
            color: #8f98a5;
        }

        /* CARDS */

        .cards {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 20px;
        }

        .card {
            background: rgba(17, 21, 28, .8);
            border: 1px solid #282f3a;
            border-radius: 12px;
            padding: 30px;
            transition: .3s;
        }

        .card:hover {
            transform: translateY(-5px);
            border-color: #555d69;
        }

        .number {
            font-size: 35px;
            color: #737b87;
            margin-bottom: 20px;
        }

        .card h3 {
            margin-bottom: 12px;
        }

        .card p {
            color: #929aa6;
            line-height: 1.9;
        }

        /* RULES */

        .rules {
            background: rgba(12, 15, 20, .7);
            border: 1px solid #282e38;
            border-radius: 14px;
            padding: 35px;
        }

        .rules li {
            list-style: none;
            padding: 17px;
            border-bottom: 1px solid #252a32;
            color: #c5cad1;
        }

        .rules li:last-child {
            border-bottom: none;
        }

        .rules li::before {
            content: "✓";
            margin-left: 12px;
            color: #aeb5bf;
        }

        /* ACTIVATION */

        .activation-box {
            background: linear-gradient(145deg, #151a22, #0c0f14);
            border: 1px solid #303743;
            border-radius: 16px;
            padding: 55px;
            text-align: center;
        }

        .activation-box h2 {
            font-size: 38px;
            margin-bottom: 15px;
        }

        .activation-box p {
            color: #9ba3ae;
            line-height: 2;
            margin-bottom: 30px;
        }

        /* FOOTER */

        footer {
            border-top: 1px solid #252b34;
            text-align: center;
            padding: 35px;
            color: #6f7782;
        }

        @media(max-width:700px) {
            nav {
                padding: 0 20px;
            }

            nav ul {
                display: none;
            }

            .hero h1 {
                letter-spacing: 3px;
            }

            .activation-box {
                padding: 30px 20px;
            }
        }
    </style>
</head>

<body>

<!-- NAVBAR -->

<nav>

    <div class="logo">
        RIFLE <span>TOWN</span>
    </div>

    <ul>
        <li><a href="#home">الرئيسية</a></li>
        <li><a href="#activation">التفعيل</a></li>
        <li><a href="#rules">القوانين</a></li>
        <li><a href="#about">عن المدينة</a></li>
    </ul>

</nav>


<!-- HERO -->

<div class="hero" id="home">

    <div class="hero-content">

        <small>WELCOME TO</small>

        <h1>ريفل تاون</h1>

        <h2>RIFLE TOWN</h2>

        <p>
            مرحباً بك في ريفل تاون
            <br>
            المدينة التي تبدأ فيها قصتك.
        </p>

        <div class="buttons">

            <a href="#activation" class="btn">
                تفعيل الحساب
            </a>

            <a href="#rules" class="btn dark">
                قراءة القوانين
            </a>

        </div>

    </div>

</div>


<!-- ABOUT -->

<section id="about">

    <div class="title">

        <h2>عن ريفل تاون</h2>

        <p>
            مجتمع رول بلاي يهتم بالتجربة والواقعية
        </p>

    </div>


    <div class="cards">

        <div class="card">

            <div class="number">01</div>

            <h3>رول بلاي</h3>

            <p>
                تجربة لعب تعتمد على تقمص الشخصية
                والتفاعل مع أحداث المدينة.
            </p>

        </div>


        <div class="card">

            <div class="number">02</div>

            <h3>مجتمع</h3>

            <p>
                مجتمع متكامل للاعبين والإداريين
                وأصحاب القطاعات.
            </p>

        </div>


        <div class="card">

            <div class="number">03</div>

            <h3>تجربة مختلفة</h3>

            <p>
                أنظمة وفعاليات وتجارب متنوعة
                داخل رايفل تاون.
            </p>

        </div>

    </div>

</section>


<!-- ACTIVATION -->

<section id="activation">

    <div class="activation-box">

        <h2>تفعيل الحساب</h2>

        <p>
            قبل دخولك إلى رايفل تاون يجب عليك
            قراءة القوانين وإكمال نموذج التفعيل.
            <br>
            بعد إرسال الطلب سيتم مراجعته من الإدارة.
        </p>

        <!-- حط رابط Google Forms هنا -->

        <a
            href="href="https://forms.google.com/...""
            target="_blank"
            class="btn">

            بدء التفعيل

        </a>

    </div>

</section>


<!-- RULES -->

<section id="rules">

    <div class="title">

        <h2>قوانين ريفل تاون</h2>

        <p>
            يجب قراءة القوانين قبل التفعيل
        </p>

    </div>


    <div class="rules">

        <ul>

            <li>
                احترام جميع اللاعبين والإدارة.
            </li>

            <li>
                الالتزام بأنظمة الرول بلاي.
            </li>

            <li>
                يمنع استخدام المعلومات التي حصلت عليها
                خارج الشخصية داخل الرول بلاي.
            </li>

            <li>
                يمنع استغلال الأخطاء أو الثغرات.
            </li>

            <li>
                الالتزام بتعليمات الإدارة.
            </li>

            <li>
                يمنع التخريب أو الإزعاج المتعمد.
            </li>

            <li>
                يجب المحافظة على تجربة لعب عادلة للجميع.
            </li>

        </ul>

    </div>

</section>


<!-- FINAL CTA -->

<section>

    <div class="activation-box">

        <h2>جاهز تبدأ قصتك؟</h2>

        <p>
            أكمل التفعيل وانضم إلى ريفل تاون.
        </p>

        <a href="#activation" class="btn">
            تفعيل الآن
        </a>

    </div>

</section>


<!-- FOOTER -->

<footer>

    © 2026 RIFLE TOWN

    <br>

    جميع الحقوق محفوظة

</footer>


</body>
</html>
