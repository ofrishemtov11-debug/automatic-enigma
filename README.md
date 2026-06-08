# automatic-enigma<!DOCTYPE html>
<html lang="he" dir="rtl">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Ofri סקווישים 🧸</title>
    <style>
        :root {
            --pink-baby: #ffb6c1;
            --pink-dark: #ff69b4;
            --bg-rainbow: linear-gradient(120deg, #fff5f5 0%, #fff0f5 100%);
            --white: #ffffff;
        }

        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            background: var(--bg-rainbow);
            margin: 0;
            padding: 0;
            color: #333;
        }

        header {
            background-color: var(--pink-baby);
            text-align: center;
            padding: 30px 20px;
            border-bottom: 5px solid #fff;
            box-shadow: 0 4px 6px rgba(0,0,0,0.05);
        }

        .logo-area h1 {
            margin: 0;
            font-size: 2.8rem;
            color: var(--pink-dark);
            text-shadow: 2px 2px #fff;
        }

        .logo-area p {
            margin: 5px 0 0 0;
            font-size: 1.2rem;
            color: #555;
        }

        main {
            max-width: 1000px;
            margin: 20px auto;
            padding: 0 20px;
        }

        section {
            background: var(--white);
            border-radius: 20px;
            padding: 25px;
            margin-bottom: 30px;
            box-shadow: 0 8px 16px rgba(0,0,0,0.04);
            border: 2px solid #ffe4e1;
        }

        h2 {
            color: var(--pink-dark);
            border-bottom: 3px dashed var(--pink-baby);
            padding-bottom: 10px;
            margin-top: 0;
        }

        /* Hero Product */
        .hero-product {
            display: flex;
            flex-direction: column;
            align-items: center;
            text-align: center;
            background: #fff0f5;
            padding: 20px;
            border-radius: 15px;
            border: 3px solid var(--pink-baby);
        }

        .hero-icon {
            font-size: 5rem;
            margin-bottom: 10px;
        }

        /* Grid Products */
        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(220px, 1fr));
            gap: 20px;
            margin-top: 20px;
        }

        .product-card {
            background: #fff;
            border: 2px solid #f0f0f0;
            border-radius: 15px;
            padding: 15px;
            text-align: center;
            transition: transform 0.2s;
            display: flex;
            flex-direction: column;
            justify-content: space-between;
        }

        .product-card:hover {
            transform: scale(1.03);
            border-color: var(--pink-baby);
        }

        .product-icon {
            font-size: 3.5rem;
            margin-bottom: 10px;
        }

        .price {
            font-size: 1.3rem;
            font-weight: bold;
            color: #2c3e50;
            margin: 10px 0;
        }

        button {
            background-color: var(--pink-dark);
            color: white;
            border: none;
            padding: 10px 20px;
            font-size: 1rem;
            border-radius: 25px;
            cursor: pointer;
            font-weight: bold;
            transition: background 0.2s;
            width: 100%;
        }

        button:hover {
            background-color: #ff1493;
        }

        /* Tips & AI */
        .tips-list, .video-placeholder {
            margin-top: 15px;
        }

        .tips-list li {
            margin-bottom: 10px;
            font-size: 1.1rem;
        }

        .video-box {
            background: #333;
            color: #fff;
            height: 200px;
            border-radius: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 1.2rem;
            margin-top: 10px;
            border: 4px solid var(--pink-baby);
        }

        /* Cart & Checkout */
        .cart-item {
            display: flex;
            justify-content: space-between;
            padding: 10px 0;
            border-bottom: 1px solid #eee;
        }

        .summary-line {
            display: flex;
            justify-content: space-between;
            font-size: 1.2rem;
            margin-top: 10px;
        }

        .total-line {
            font-weight: bold;
            color: var(--pink-dark);
            font-size: 1.4rem;
            border-top: 2px solid var(--pink-baby);
            padding-top: 10px;
        }

        .checkout-form {
            margin-top: 20px;
            background: #fdf6f6;
            padding: 15px;
            border-radius: 10px;
        }

        .checkout-form input {
            width: 100%;
            padding: 10px;
            margin: 8px 0;
            box-sizing: border-box;
            border: 2px solid var(--pink-baby);
            border-radius: 8px;
            font-size: 1rem;
            text-align: center;
        }

        /* Modal Popup */
        .modal {
            display: none;
            position: fixed;
            top: 0; left: 0; width: 100%; height: 100%;
            background: rgba(0,0,0,0.6);
            justify-content: center;
            align-items: center;
            z-index: 1000;
        }

        .modal-content {
            background: white;
            padding: 40px;
            border-radius: 20px;
            text-align: center;
            max-width: 500px;
            margin: 20px;
            border: 5px solid var(--pink-baby);
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
        }

        .modal-content h3 {
            color: var(--pink-dark);
            font-size: 2rem;
            margin-top: 0;
        }

        .modal-content p {
            font-size: 1.2rem;
            line-height: 1.6;
        }

        .close-btn {
            background: #333;
            margin-top: 20px;
            width: auto;
        }
    </style>
</head>
<body>

    <header>
        <div class="logo-area">
            <h1>🧸 Ofri סקווישים 🧸</h1>
            <p>חנות הסקווישים הכי מתוקה ברשת (במצב בדיקה!)</p>
        </div>
    </header>

    <main>
        <!-- קטגוריה 1: טרנדים -->
        <section id="trends">
            <h2>🔥 הטרנדים הכי חמים של עופרי</h2>
            
            <!-- בקדמת הבמה -->
            <div class="hero-product">
                <div class="hero-icon">☁️🦄🧸</div>
                <h3>👑 סקוויש ענקי בטירוף!</h3>
                <p>עם קצף בטוח, סופר-סלואו רייז ומפנק ברמות בפנים!</p>
                <div class="price">50 ש"ח</div>
                <button onclick="addToCart('סקוויש ענקי בטירוף', 50)">[להוספה לסל]</button>
            </div>

            <!-- גלריית הטרנדים -->
            <div class="products-grid">
                <div class="product-card">
                    <div class="product-icon">🐱☁️</div>
                    <h3>סקוויש חתלתול ישן על ענן</h3>
                    <div class="price">35 ש"ח</div>
                    <button onclick="addToCart('סקוויש חתלתול על ענן', 35)">[להוספה לסל]</button>
                </div>
                <div class="product-card">
                    <div class="product-icon">🧋</div>
                    <h3>סקוויש כוס תה בועות (בובה טי)</h3>
                    <div class="price">32 ש"ח</div>
                    <button onclick="addToCart('סקוויש בובה טי', 32)">[להוספה לסל]</button>
                </div>
                <div class="product-card">
                    <div class="product-icon">🧁🍓</div>
                    <h3>סקוויש קאפקייק קצפת תות</h3>
                    <div class="price">25 ש"ח</div>
                    <button onclick="addToCart('סקוויש קאפקייק תות', 25)">[להוספה לסל]</button>
                </div>
                <div class="product-card">
                    <div class="product-icon">🥑😊</div>
                    <h3>סקוויש חצי אבוקדו מחייך</h3>
                    <div class="price">22 ש"ח</div>
                    <button onclick="addToCart('סקוויש אבוקדו מחייך', 22)">[להוספה לסל]</button>
                </div>
                <div class="product-card">
                    <div class="product-icon">🍩🌈</div>
                    <h3>סקוויש דונאטס עם סוכריות</h3>
                    <div class="price">20 ש"ח</div>
                    <button onclick="addToCart('סקוויש דונאטס צבעוני', 20)">[להוספה לסל]</button>
                </div>
                <div class="product-card">
                    <div class="product-icon">🐥💛</div>
                    <h3>סקוויש אפרוח צהוב קטנטן</h3>
                    <div class="price">10 ש"ח</div>
                    <button onclick="addToCart('סקוויש אפרוח קטנטן', 10)">[להוספה לסל]</button>
                </div>
            </div>
        </section>

        <!-- קטגוריה 2: טיפים וסרטונים -->
        <section id="content">
            <h2>🎬 פינת ה-AI והטיפים של עופרי</h2>
            <div class="video-placeholder">
                <h3>🤖 סרטוני ה-AI של עופרי:</h3>
                <div class="video-box">
                    🎬 [כאן הסקווישים קמים לחיים, רוקדים ומדברים!]
                </div>
            </div>
            <div class="tips-list">
                <h3>💡 הטיפים של עופרי לשמירה על הסקוויש:</h3>
                <ul>
                    <li>אל תלחצו על הסקוויש הענקי עם ציפורניים חדות כדי לשמור על הקצף שבפנים. ✨</li>
                    <li>אם הסקוויש התלכלך, שטפו אותו בעדינות עם מים פושרים וקצת סבון. 🧼</li>
                </ul>
            </div>
        </section>

        <!-- קטגוריה 3: עגלת קניות והזמנה דמיונית -->
        <section id="cart-section">
            <h2>🛍️ עגלת הקניות שלכם (סימולציית בדיקה)</h2>
            <div id="cart-items-container">
                <p style="text-align: center; color: #777;">העגלה שלכם ריקה. תתחילו להוסיף סקווישים! 🛒</p>
            </div>
            
            <div class="summary-line">
