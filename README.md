# FreshEgg-Direct
FreshEgg Direct - Fresh eggs with reliable delivery at fair prices.
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>FreshEgg Direct | Fresh Eggs Delivered</title>

    <meta name="description"
          content="FreshEgg Direct delivers fresh, quality eggs to businesses at fair prices with reliable service.">

    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            scroll-behavior: smooth;
        }

        body {
            font-family: Arial, Helvetica, sans-serif;
            color: #333;
            background: #fffdf7;
            line-height: 1.6;
        }

        /* NAVBAR */
        header {
            background: #ffffff;
            padding: 18px 7%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
            box-shadow: 0 2px 10px rgba(0,0,0,0.08);
        }

        .logo {
            font-size: 25px;
            font-weight: bold;
            color: #d97706;
        }

        .logo span {
            color: #333;
        }

        nav a {
            text-decoration: none;
            color: #333;
            margin-left: 25px;
            font-weight: 600;
        }

        nav a:hover {
            color: #d97706;
        }

        /* HERO */
        .hero {
            min-height: 85vh;
            display: flex;
            align-items: center;
            justify-content: space-between;
            padding: 60px 8%;
            background: linear-gradient(135deg, #fff7d6, #fffdf7);
            gap: 40px;
        }

        .hero-text {
            max-width: 600px;
        }

        .hero-text h1 {
            font-size: 55px;
            line-height: 1.15;
            margin-bottom: 20px;
            color: #222;
        }

        .hero-text h1 span {
            color: #d97706;
        }

        .hero-text p {
            font-size: 19px;
            color: #555;
            margin-bottom: 30px;
        }

        .buttons {
            display: flex;
            gap: 15px;
            flex-wrap: wrap;
        }

        .btn {
            display: inline-block;
            padding: 14px 25px;
            border-radius: 8px;
            text-decoration: none;
            font-weight: bold;
            transition: 0.3s;
        }

        .primary {
            background: #d97706;
            color: white;
        }

        .primary:hover {
            background: #b45309;
            transform: translateY(-2px);
        }

        .secondary {
            border: 2px solid #d97706;
            color: #d97706;
        }

        .secondary:hover {
            background: #d97706;
            color: white;
        }

        /* EGG ILLUSTRATION */
        .egg-area {
            width: 350px;
            height: 350px;
            display: flex;
            align-items: center;
            justify-content: center;
        }

        .egg {
            width: 230px;
            height: 290px;
            background: white;
            border-radius: 50% 50% 48% 48%;
            box-shadow: 0 15px 35px rgba(0,0,0,0.15);
            position: relative;
            transform: rotate(-5deg);
        }

        .yolk {
            position: absolute;
            width: 100px;
            height: 100px;
            background: #f59e0b;
            border-radius: 50%;
            top: 95px;
            left: 65px;
            box-shadow: inset 0 -8px 10px rgba(180,90,0,0.15);
        }

        /* SECTIONS */
        section {
            padding: 80px 8%;
        }

        .section-title {
            text-align: center;
            margin-bottom: 45px;
        }

        .section-title h2 {
            font-size: 38px;
            color: #222;
            margin-bottom: 10px;
        }

        .section-title p {
            color: #666;
        }

        /* FEATURES */
        .features {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .card {
            background: white;
            padding: 30px;
            border-radius: 15px;
            text-align: center;
            box-shadow: 0 5px 20px rgba(0,0,0,0.07);
            transition: 0.3s;
        }

        .card:hover {
            transform: translateY(-7px);
        }

        .icon {
            font-size: 45px;
            margin-bottom: 15px;
        }

        .card h3 {
            margin-bottom: 10px;
            color: #222;
        }

        .card p {
            color: #666;
        }

        /* PRODUCTS */
        #products {
            background: #fff7d6;
        }

        .products {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 25px;
        }

        .product {
            background: white;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 5px 20px rgba(0,0,0,0.08);
            text-align: center;
            padding-bottom: 25px;
        }

        .product-image {
            height: 180px;
            display: flex;
            align-items: center;
            justify-content: center;
            background: #fffdf7;
            font-size: 80px;
        }

        .product h3 {
            margin: 20px 0 5px;
        }

        .price {
            font-size: 22px;
            font-weight: bold;
            color: #d97706;
            margin: 10px;
        }

        /* ABOUT */
        .about {
            display: flex;
            align-items: center;
            gap: 60px;
        }

        .about-text {
            flex: 1;
        }

        .about-text h2 {
            font-size: 38px;
            margin-bottom: 20px;
        }

        .about-text p {
            color: #555;
            margin-bottom: 15px;
        }

        .about-box {
            flex: 1;
            background: #fff7d6;
            padding: 40px;
            border-radius: 20px;
        }

        .about-box h3 {
            margin-bottom: 15px;
            color: #d97706;
        }

        /* CONTACT */
        #contact {
            background: #222;
            color: white;
        }

        .contact-container {
            max-width: 800px;
            margin: auto;
            text-align: center;
        }

        .contact-container h2 {
            font-size: 38px;
            margin-bottom: 15px;
        }

        .contact-container p {
            color: #ddd;
            margin-bottom: 25px;
        }

        .contact-info {
            display: flex;
            justify-content: center;
            gap: 25px;
            flex-wrap: wrap;
            margin-top: 25px;
        }

        .contact-item {
            background: #333;
            padding: 15px 25px;
            border-radius: 8px;
        }

        .contact-item a {
            color: #ffd166;
            text-decoration: none;
        }

        /* FOOTER */
        footer {
            background: #111;
            color: #aaa;
            text-align: center;
            padding: 25px;
        }

        footer span {
            color: #f59e0b;
        }

        /* MOBILE */
        @media (max-width: 850px) {

            header {
                flex-direction: column;
                gap: 15px;
            }

            nav a {
                margin: 0 8px;
                font-size: 14px;
            }

            .hero {
                flex-direction: column;
                text-align: center;
                padding-top: 50px;
            }

            .hero-text h1 {
                font-size: 42px;
            }

            .buttons {
                justify-content: center;
            }

            .features,
            .products {
                grid-template-columns: 1fr;
            }

            .about {
                flex-direction: column;
            }

            .egg-area {
                width: 280px;
                height: 280px;
            }
        }
    </style>
</head>

<body>

<!-- NAVBAR -->
<header>

    <div class="logo">
        🥚 FreshEgg <span>Direct</span>
    </div>

    <nav>
        <a href="#home">Home</a>
        <a href="#products">Products</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
    </nav>

</header>


<!-- HERO -->
<section class="hero" id="home">

    <div class="hero-text">

        <h1>
            Fresh Eggs.<br>
            <span>Fair Prices.</span><br>
            Reliable Delivery.
        </h1>

        <p>
            FreshEgg Direct delivers fresh, quality eggs to businesses
            with reliable service and fair prices.
        </p>

        <div class="buttons">

            <a href="#products" class="btn primary">
                View Products
            </a>

            <a href="#contact" class="btn secondary">
                Contact Us
            </a>

        </div>

    </div>


    <div class="egg-area">

        <div class="egg">

            <div class="yolk"></div>

        </div>

    </div>

</section>


<!-- WHY US -->
<section>

    <div class="section-title">

        <h2>Why FreshEgg Direct?</h2>

        <p>
            Quality eggs and dependable service for your business.
        </p>

    </div>


    <div class="features">

        <div class="card">

            <div class="icon">🥚</div>

            <h3>Fresh Quality</h3>

            <p>
                We focus on supplying fresh and quality eggs
                for your business.
            </p>

        </div>


        <div class="card">

            <div class="icon">💰</div>

            <h3>Fair Prices</h3>

            <p>
                Competitive pricing helps businesses manage
                their costs effectively.
            </p>

        </div>


        <div class="card">

            <div class="icon">🚚</div>

            <h3>Reliable Delivery</h3>

            <p>
                Dependable delivery service designed around
                your regular business needs.
            </p>

        </div>

    </div>

</section>


<!-- PRODUCTS -->
<section id="products">

    <div class="section-title">

        <h2>Our Products</h2>

        <p>
            Choose the egg supply that fits your business.
        </p>

    </div>


    <div class="products">

        <div class="product">

            <div class="product-image">
                🥚🥚🥚
            </div>

            <h3>Fresh White Eggs</h3>

            <p>
                Fresh eggs suitable for regular business supply.
            </p>

            <div class="price">
                Contact for Price
            </div>

            <a href="#contact" class="btn primary">
                Enquire Now
            </a>

        </div>


        <div class="product">

            <div class="product-image">
                🥚🥚🥚
            </div>

            <h3>Fresh Brown Eggs</h3>

            <p>
                Quality brown eggs for shops and businesses.
            </p>

            <div class="price">
                Contact for Price
            </div>

            <a href="#contact" class="btn primary">
                Enquire Now
            </a>

        </div>


        <div class="product">

            <div class="product-image">
                📦🥚
            </div>

            <h3>Bulk Egg Supply</h3>

            <p>
                Bulk supply options for businesses with regular demand.
            </p>

            <div class="price">
                Custom Pricing
            </div>

            <a href="#contact" class="btn primary">
                Enquire Now
            </a>

        </div>

    </div>

</section>


<!-- ABOUT -->
<section id="about">

    <div class="about">

        <div class="about-text">

            <h2>About FreshEgg Direct</h2>

            <p>
                FreshEgg Direct is focused on making fresh egg
                supply simple and reliable for businesses.
            </p>

            <p>
                Our goal is to connect businesses with quality
                eggs at fair prices while providing dependable
                service.
            </p>

            <p>
                Whether you run a grocery shop or another
                business that regularly needs eggs, FreshEgg
                Direct is designed to make ordering easier.
            </p>

        </div>


        <div class="about-box">

            <h3>Our Mission</h3>

            <p>
                To provide businesses with fresh, quality eggs
                at fair prices through reliable and convenient
                delivery.
            </p>

            <br>

            <h3>Who We Serve</h3>

            <p>
                🏪 Grocery Shops<br>
                🍽️ Food Businesses<br>
                🏨 Hotels<br>
                🏢 Other Local Businesses
            </p>

        </div>

    </div>

</section>


<!-- CONTACT -->
<section id="contact">

    <div class="contact-container">

        <h2>Let's Work Together</h2>

        <p>
            Need a reliable egg supplier for your business?
            Get in touch with FreshEgg Direct.
        </p>

        <a
            href="mailto:your-email@example.com"
            class="btn primary">
            Contact Us
        </a>


        <div class="contact-info">

            <div class="contact-item">
                📧
                <a href="mailto:your-email@example.com">
                    Email Us
                </a>
            </div>

            <div class="contact-item">
                📞
                <a href="tel:+910000000000">
                    Call Us
                </a>
            </div>

        </div>

    </div>

</section>


<!-- FOOTER -->
<footer>

    <p>
        © 2026 <span>FreshEgg Direct</span>.
        All rights reserved.
    </p>

    <p>
        Fresh eggs • Fair prices • Reliable delivery
    </p>

</footer>

</body>
</html>
```
