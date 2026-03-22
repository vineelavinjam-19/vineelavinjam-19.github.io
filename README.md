<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">

<title>Madhurakshi</title>

<link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500;700&family=Poppins:wght@300;400;500&display=swap" rel="stylesheet">

<style>

/* ===== GLOBAL IMAGE SIZE ===== */
img {
    width: 100%;
    height: 300px;
    object-fit: cover;
    border-radius: 10px;
}

.slides img { height: 400px; }
.cat-card img { height: 250px; }
.card img { height: 300px; }
.insta-grid img { height: 200px; }

/* ===== NAVBAR ===== */
.navbar {
    display: flex;
    justify-content: space-between;
    padding: 15px 40px;
    background: #fff;
    position: sticky;
    top: 0;
}

.logo {
    font-size: 24px;
    font-weight: bold;
    color: #b3002d;
}

.nav-links a {
    margin-left: 20px;
    text-decoration: none;
    color: #333;
}

/* ===== HERO ===== */
.hero-premium {
    display: flex;
    align-items: center;
    justify-content: space-between;
    padding: 80px 60px;
    background: #f5e6d3;
}

.hero-text {
    width: 50%;
}

.hero-text h1 {
    font-family: 'Playfair Display', serif;
    font-size: 42px;
    line-height: 1.4;
    color: #8b5e3c;
    font-weight: 600;
}

.hero-image {
    width: 40%;
    text-align: center;
}

.hero-image img {
    width: 80%;
    max-height: 400px;
    object-fit: contain;
}

/* ===== BUTTON ===== */
.btn {
    background: #b3002d;
    color: white;
    padding: 12px 25px;
    border-radius: 5px;
    text-decoration: none;
    display: inline-block;
}

/* ===== SECTION ===== */
.section {
    padding: 60px 40px;
    text-align: center;
}

/* ===== SLIDER ===== */
.slider {
    overflow: hidden;
    max-width: 900px;
    margin: auto;
}

.slides {
    display: flex;
    animation: slide 12s infinite;
}

.slides img {
    width: 100%;
    border-radius: 10px;
    margin: 10px;
}

@keyframes slide {
    0% {transform: translateX(0);}
    33% {transform: translateX(-100%);}
    66% {transform: translateX(-200%);}
    100% {transform: translateX(0);}
}

/* ===== COLLECTIONS ===== */
.categories {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(180px, 1fr));
    gap: 20px;
}

.cat-card {
    background: white;
    border-radius: 10px;
    overflow: hidden;
    transition: 0.3s;
}

.cat-card:hover {
    transform: scale(1.05);
}

/* ===== PRODUCTS ===== */
.products {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
}

.card {
    background: white;
    padding: 15px;
    border-radius: 10px;
    position: relative;
}

/* SOLD OUT BADGE */
.sold-out {
    position: absolute;
    top: 15px;
    left: 15px;
    background: #b3002d;
    color: white;
    width: 70px;
    height: 70px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 12px;
    font-weight: bold;
    text-align: center;
}

/* optional grey effect */
.sold img {
    filter: grayscale(60%);
    opacity: 0.7;
}

/* ===== INSTAGRAM ===== */
.insta-grid {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 10px;
}

/* ===== FOOTER ===== */
.footer {
    background: white;
    padding: 20px;
    text-align: center;
}

</style>
</head>

<body>

<!-- NAVBAR -->
<div class="navbar">
    <div class="logo">Madhurakshi</div>
    <div class="nav-links">
        <a href="#">Home</a>
        <a href="#collection">Collections</a>
        <a href="#contact">Contact</a>
    </div>
</div>

<!-- HERO -->
<div class="hero-premium">
    <div class="hero-text">
        <h1>
            Madhurakshi is for the grace she carries,  
            the stories she weaves, and the elegance she becomes.
        </h1>

        <a href="#collection" class="btn">Explore Collection</a>
        <br><br>
        <a href="https://www.instagram.com/madhurakshiofficial" target="_blank" class="btn">
            Order via Instagram 📩
        </a>
    </div>

    <div class="hero-image">
        <img src="logo.png">
    </div>
</div>

<!-- NEW COLLECTION -->
<div class="section">
    <h2>New Collection ✨</h2>
    <div class="slider">
        <div class="slides">
            <img src="https://images.unsplash.com/photo-1583391733956-6c78276477e2">
            <img src="https://images.unsplash.com/photo-1602810318383-e386cc2a3ccf">
            <img src="https://images.unsplash.com/photo-1618354691373-d851c5c3a990">
        </div>
    </div>
</div>

<!-- COLLECTION TYPES -->
<div class="section" id="collection">
    <h2>Shop by Collection</h2>
    <div class="categories">
        <div class="cat-card"><img src="https://images.unsplash.com/photo-1602810318383-e386cc2a3ccf"><h3>Lehengas</h3></div>
        <div class="cat-card"><img src="https://images.unsplash.com/photo-1583391733956-6c78276477e2"><h3>Anarkali</h3></div>
        <div class="cat-card"><img src="https://images.unsplash.com/photo-1618354691373-d851c5c3a990"><h3>Kurthi</h3></div>
    </div>
</div>

<!-- BESTSELLERS -->
<div class="section">
    <h2>Bestsellers</h2>

    <div class="products">

        <!-- SOLD OUT PRODUCT -->
        <div class="card sold">
            <div class="sold-out">SOLD OUT</div>
            <img src="https://images.unsplash.com/photo-1593032465171-8d1d6a8f9b10">
            <h3>Signature Anarkali</h3>
        </div>

        <!-- NORMAL PRODUCT -->
        <div class="card">
            <img src="/Users/vineelavinjam/Downloads/_ (2).jpeg">
            <h3>Festive Lehenga</h3>
            <!-- class="card sold" -->
            <div class="sold-out">SOLD OUT</div>
        </div>

        <!-- NORMAL PRODUCT -->
        <div class="card">
            <img src="https://images.unsplash.com/photo-1618354691373-d851c5c3a990">
            <h3>Classic Kurthi</h3>
        </div>

    </div>
</div>

<!-- CONTACT -->
<div class="section" id="contact">
    <h2>Order Now</h2>
    <p>DM us on Instagram</p>
    <a href="https://instagram.com/madhurakshiofficial" target="_blank" class="btn">
        Open Instagram
    </a>
</div>

<!-- FOOTER -->
<div class="footer">
    © 2026 Madhurakshi ✨
</div>

</body>
</html>
