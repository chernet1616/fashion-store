<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Chuchu Fashion Store</title>

    <style>
        body {<section style="padding:25px;background:#f7f4ee;color:#222;border-radius:12px;margin:20px 0;">
  <h2>💳 Payment Options</h2>
  <p>Choose your preferred payment method.</p><label for="payment">Select Payment Method:</label>
<select id="payment" style="display:block;width:100%;padding:12px;margin:12px 0;">
<option value="">-- Select Payment --</option>
<option value="cbe">Commercial Bank of Ethiopia (CBE)</option>
<option value="abyssinia">Bank of Abyssinia</option>
<option value="awash">Awash Bank</option>
<option value="dashen">Dashen Bank</option>
<option value="telebirr">Telebirr</option>
<option value="mpesa">M-PESA Ethiopia</option>
</select>

  <p id="payment-info">
    Select a payment method to see the next steps.
  </p>
</section><script>
document.getElementById("payment").addEventListener("change", function () {
  const info = {
    cbe: "Please contact CHUCHU FASHION to receive official CBE payment instructions.",
    abyssinia: "Please contact CHUCHU FASHION to receive official Bank of Abyssinia payment instructions.",
    awash: "Please contact CHUCHU FASHION to receive official Awash Bank payment instructions.",
    dashen: "Please contact CHUCHU FASHION to receive official Dashen Bank payment instructions.",
    telebirr: "Please contact CHUCHU FASHION for official Telebirr payment instructions.",
    mpesa: "Please contact CHUCHU FASHION for official M-PESA payment instructions."
  };

  document.getElementById("payment-info").textContent =
    info[this.value] || "Select a payment method to see the next steps.";
});
</script>
            margin: 0;
            font-family: Arial, sans-serif;
            background: #fffaf7;
            color: #222;
        }

        header {
            background: #222;
            color: white;
            text-align: center;
            padding: 25px;
        }

        nav {
            background: #d4a373;
            padding: 15px;
            text-align: center;
        }

        nav a {
            color: white;
            text-decoration: none;
            margin: 12px;
            font-weight: bold;
        }

        .hero {
            text-align: center;
            padding: 60px 20px;
        }

        .hero h2 {
            font-size: 35px;
        }

        .products {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            gap: 20px;
            padding: 20px;
        }

        .product {
            background: white;
            width: 250px;
            padding: 15px;
            text-align: center;
            border-radius: 10px;
        }

        .product img {
            width: 100%;
            height: 260px;
            object-fit: cover;
        }

        button {
            background: #222;
            color: white;
            padding: 12px 20px;
            border: none;
            cursor: pointer;
        }

        footer {
            background: #222;
            color: white;
            padding: 20px;
            text-align: center;
        }
    </style>
</head>

<body>

    <header>
        <h1>CHUCHU FASHION</h1>
        <p>Your Style, Your Identity</p>
    </header>

    <nav>
        <a href="#home">Home</a>
        <a href="#products">Products</a>
        <a href="#gallery">Gallery</a>
        <a href="#contact">Contact</a>
    </nav>

    <section class="hero" id="home">
        <h2>Welcome to Our Fashion Store</h2>
        <p>Discover your favorite fashion styles.</p>
        <button onclick="showMessage()">Explore Store</button>
    </section>

    <section id="products">
        <h2 style="text-align:center;">Our Products</h2>

        <div class="products">

            <div class="product">
                <img src="https://placehold.co/300x350?text=Suit"
                     alt="Fashion suit">
                <h3>Classic Suit</h3>
                <p>Elegant and modern style.</p>
                <button onclick="showMessage()">View Product</button>
            </div>

            <div class="product">
                <img src="https://placehold.co/300x350?text=Shirt"
                     alt="Fashion shirt">
                <h3>Classic Shirt</h3>
                <p>Simple and stylish.</p>
                <button onclick="showMessage()">View Product</button>
            </div>

            <div class="product">
                <img src="https://placehold.co/300x350?text=Jacket"
                     alt="Fashion jacket">
                <h3>Fashion Jacket</h3>
                <p>Look smart every day.</p>
                <button onclick="showMessage()">View Product</button>
            </div>

        </div>
    </section>

    <section id="gallery" class="hero">
        <h2>Our Gallery</h2>
        <p>Discover the latest fashion collection.</p>
    </section>

    <section id="contact" class="hero">
        <h2>Contact Us</h2>
        <p>Email: yourstore@example.com</p>
    </section>

    <footer>
        <p>© 2026 Chuchu Fashion Store</p>
    </footer>

    <script>
        function showMessage() {
            alert("Welcome to Chuchu Fashion Store!");
        }
    </script>

</body>
</html>
