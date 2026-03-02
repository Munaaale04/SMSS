<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aroma Bliss - Perfumes & Fragrance Oils</title>
    <!-- Google Fonts -->
    <link href="https://fonts.googleapis.com/css2?family=Pacifico&family=Roboto:wght@400;700&display=swap" rel="stylesheet">
    <style>
        /* GENERAL STYLES */
        body {
            margin: 0;
            font-family: 'Roboto', sans-serif;
            background: linear-gradient(to right, #fff5f7, #fffefc);
            color: #333;
        }

        /* HEADER */
        header {
            background-color: #ffb6c1;
            padding: 2rem 1rem;
            text-align: center;
            color: white;
            font-family: 'Pacifico', cursive;
            box-shadow: 0 4px 6px rgba(0,0,0,0.1);
        }
        header h1 {
            margin: 0;
            font-size: 3rem;
        }
        header p {
            margin-top: 0.5rem;
            font-size: 1.2rem;
            font-weight: 400;
        }

        /* NAVIGATION */
        nav {
            display: flex;
            justify-content: center;
            background-color: #ffc0cb;
            padding: 1rem;
        }
        nav a {
            text-decoration: none;
            color: white;
            font-weight: bold;
            margin: 0 1.5rem;
            transition: color 0.3s, transform 0.3s;
        }
        nav a:hover {
            color: #ff69b4;
            transform: scale(1.1);
        }

        /* HERO SECTION */
        .hero {
            text-align: center;
            padding: 4rem 1rem;
        }
        .hero h2 {
            font-size: 2.5rem;
            color: #ff1493;
        }
        .hero p {
            font-size: 1.2rem;
            color: #555;
            max-width: 600px;
            margin: 1rem auto;
        }

        /* PRODUCTS */
        .products {
            display: flex;
            justify-content: center;
            flex-wrap: wrap;
            gap: 2rem;
            padding: 2rem;
        }
        .product-card {
            background-color: white;
            border-radius: 15px;
            width: 250px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.1);
            text-align: center;
            transition: transform 0.3s, box-shadow 0.3s;
        }
        .product-card:hover {
            transform: translateY(-10px);
            box-shadow: 0 15px 30px rgba(0,0,0,0.2);
        }
        .product-card img {
            width: 100%;
            border-top-left-radius: 15px;
            border-top-right-radius: 15px;
        }
        .product-card h3 {
            color: #ff1493;
            margin: 0.5rem 0;
        }
        .product-card p {
            padding: 0 1rem 1rem;
            color: #555;
        }
        .product-card button {
            background-color: #ff1493;
            color: white;
            border: none;
            padding: 0.5rem 1rem;
            margin-bottom: 1rem;
            border-radius: 25px;
            cursor: pointer;
            transition: background-color 0.3s;
        }
        .product-card button:hover {
            background-color: #ff69b4;
        }

        /* ABOUT SECTION */
        .about {
            background-color: #ffe6f0;
            padding: 3rem 1rem;
            text-align: center;
        }
        .about h2 {
            color: #ff1493;
        }
        .about p {
            max-width: 600px;
            margin: 1rem auto;
            color: #555;
        }

        /* CONTACT SECTION */
        .contact {
            text-align: center;
            padding: 3rem 1rem;
        }
        .contact h2 {
            color: #ff1493;
        }
        .contact form {
            max-width: 400px;
            margin: 1rem auto;
            display: flex;
            flex-direction: column;
            gap: 1rem;
        }
        .contact input, .contact textarea {
            padding: 0.8rem;
            border-radius: 10px;
            border: 1px solid #ccc;
            font-size: 1rem;
        }
        .contact button {
            background-color: #ff1493;
            color: white;
            border: none;
            padding: 0.8rem;
            border-radius: 25px;
            cursor: pointer;
            font-size: 1rem;
            transition: background-color 0.3s;
        }
        .contact button:hover {
            background-color: #ff69b4;
        }

        /* FOOTER */
        footer {
            background-color: #ffb6c1;
            color: white;
            text-align: center;
            padding: 1rem;
            margin-top: 2rem;
        }

    </style>
</head>
<body>

    <header>
        <h1>Aroma Bliss</h1>
        <p>Perfumes & Fragrance Oils for Every Mood</p>
    </header>

    <nav>
        <a href="#products">Products</a>
        <a href="#about">About</a>
        <a href="#contact">Contact</a>
    </nav>

    <section class="hero">
        <h2>Experience the Luxury of Aroma</h2>
        <p>Discover the finest perfumes and essential fragrance oils, carefully crafted to elevate your senses and enrich every moment.</p>
    </section>

    <section class="products" id="products">
        <!-- Product 1 -->
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1587574293340-b49030ee60c0?auto=format&fit=crop&w=800&q=80" alt="Lavender Perfume">
            <h3>Lavender Perfume</h3>
            <p>A calming fragrance with the soothing essence of fresh lavender fields.</p>
            <button onclick="buyNow('Lavender Perfume')">Buy Now</button>
        </div>

        <!-- Product 2 -->
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1600185369760-7cfc01908f32?auto=format&fit=crop&w=800&q=80" alt="Rose Oil">
            <h3>Rose Oil</h3>
            <p>Romantic and elegant, perfect for special occasions or daily luxury.</p>
            <button onclick="buyNow('Rose Oil')">Buy Now</button>
        </div>

        <!-- Product 3 -->
        <div class="product-card">
            <img src="https://images.unsplash.com/photo-1592595896833-2e0f0f653c24?auto=format&fit=crop&w=800&q=80" alt="Vanilla Perfume">
            <h3>Vanilla Perfume</h3>
            <p>Sweet and warm aroma that leaves a lasting impression.</p>
            <button onclick="buyNow('Vanilla Perfume')">Buy Now</button>
        </div>
    </section>

    <section class="about" id="about">
        <h2>About Aroma Bliss</h2>
        <p>Aroma Bliss is dedicated to creating premium perfumes and fragrance oils, blending nature's finest essences to bring harmony, relaxation, and joy into your everyday life. Every scent tells a story.</p>
    </section>

    <section class="contact" id="contact">
        <h2>Contact Us</h2>
        <form onsubmit="submitForm(event)">
            <input type="text" placeholder="Your Name" required>
            <input type="email" placeholder="Your Email" required>
            <textarea placeholder="Your Message" rows="4" required></textarea>
            <button type="submit">Send Message</button>
        </form>
    </section>

    <footer>
        &copy; 2026 Aroma Bliss | All Rights Reserved
    </footer>

    <script>
        function buyNow(productName) {
            alert(`Thank you for choosing ${productName}! Proceeding to purchase...`);
        }

        function submitForm(event) {
            event.preventDefault();
            alert("Thank you for contacting Aroma Bliss! We will reach out to you soon.");
        }
    </script>

</body>
</html>
