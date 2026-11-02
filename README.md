# Commercial-Website-using-Flexbox
# Ex02 Commercial Website
## Date:2-11-2026

## AIM
To create a commercial website using CSS Flexbox.

## ALGORITHM
### STEP 1
Create an HTML file (index.html)

### STEP 2
Create a CSS file (style.css)

### STEP 3
Include a navigation bar with links to different sections.

### STEP 4
Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

### STEP 5
Include social media links at the footer with copyright information.

### STEP 6
Define global styles for fonts, colors, and layout.

### STEP 7
Style the header, navigation bar, and sections.

### STEP 8
Use Flexbox for layout design.

### STEP 9
Add hover effects and transitions for interactivity.

### STEP 10
Add Images and Media.

### STEP 11
Use optimized images for a professional look.

### STEP 12
Open the HTML file in a browser to check layout and functionality.

### STEP 13
Fix styling issues and refine content placement.

### STEP 14
Deploy the website.

### STEP 15
Upload to GitHub Pages for free hosting.

## PROGRAM
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Sakura Bloom Cafe</title>

<style>
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Georgia, serif;
    background-color: #fff5f7;
    color: #543b40;
}

/* Navigation */
header {
    background-color: #f7dce5;
    padding: 20px 8%;
}

nav {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
}

.logo {
    font-size: 28px;
    color: #a74768;
    font-weight: bold;
}

nav ul {
    display: flex;
    gap: 25px;
    list-style: none;
    flex-wrap: wrap;
}

nav ul a {
    text-decoration: none;
    color: #633d4b;
    font-size: 17px;
}

nav ul a:hover {
    color: #d45b86;
}

/* Hero Section */
.hero {
    min-height: 500px;
    background:
    linear-gradient(rgba(60,20,35,0.35),
    rgba(60,20,35,0.35)),
    url("https://images.unsplash.com/photo-1528360983277-13d401cdc186?w=1400")
    center/cover;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 40px;
    color: white;
}

.hero-content h1 {
    font-size: 55px;
    margin-bottom: 15px;
}

.hero-content p {
    font-size: 21px;
    margin-bottom: 25px;
}

.btn {
    background-color: #d96b91;
    color: white;
    padding: 13px 30px;
    text-decoration: none;
    border-radius: 25px;
    display: inline-block;
}

.btn:hover {
    background-color: #a74768;
}

/* About */
.about {
    padding: 60px 8%;
    text-align: center;
}

.about h2, .menu h2 {
    font-size: 35px;
    color: #a74768;
    margin-bottom: 20px;
}

.about p {
    font-size: 18px;
    line-height: 1.8;
    max-width: 750px;
    margin: auto;
}

/* Menu */
.menu {
    padding: 60px 8%;
    background-color: #fce8ee;
    text-align: center;
}

.products {
    display: flex;
    justify-content: center;
    align-items: stretch;
    flex-wrap: wrap;
    gap: 25px;
    margin-top: 35px;
}

.card {
    background-color: white;
    width: 260px;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 5px 15px #d9b9c3;
    transition: transform 0.3s;
}

.card:hover {
    transform: translateY(-8px);
}

.card img {
    width: 100%;
    height: 190px;
    object-fit: cover;
}

.card h3 {
    color: #a74768;
    margin: 15px 0 8px;
}

.card p {
    padding: 0 15px;
    margin-bottom: 10px;
}

.price {
    color: #d45b86;
    font-weight: bold;
    font-size: 19px;
    padding-bottom: 20px;
}

/* Special section */
.special {
    padding: 60px 8%;
    text-align: center;
}

.special h2 {
    color: #a74768;
    font-size: 32px;
    margin-bottom: 15px;
}

/* Footer */
footer {
    background-color: #543b40;
    color: white;
    padding: 35px 8%;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    gap: 25px;
}

.footer-content h3 {
    color: #ffb8cf;
    margin-bottom: 12px;
}

footer p {
    line-height: 1.8;
}

.copyright {
    text-align: center;
    margin-top: 25px;
    border-top: 1px solid #97727e;
    padding-top: 20px;
}

/* Responsive Design */
@media (max-width: 600px) {
    nav {
        flex-direction: column;
    }

    nav ul {
        justify-content: center;
        gap: 15px;
    }

    .hero-content h1 {
        font-size: 35px;
    }

    .hero-content p {
        font-size: 17px;
    }

    .card {
        width: 100%;
        max-width: 350px;
    }

    .footer-content {
        flex-direction: column;
        text-align: center;
    }
}
</style>
</head>

<body>

<!-- Navigation -->
<header>
<nav>
    <div class="logo">🌸 Sakura Bloom</div>
    <ul>
        <li><a href="#home">Home</a></li>
        <li><a href="#about">About</a></li>
        <li><a href="#menu">Menu</a></li>
        <li><a href="#contact">Contact</a></li>
    </ul>
</nav>
</header>

<!-- Hero -->
<section class="hero" id="home">
<div class="hero-content">
    <h1>Welcome to Sakura Bloom</h1>
    <p>Experience the beauty of Japan, one sip at a time.</p>
    <a href="#menu" class="btn">Explore Our Menu</a>
</div>
</section>

<!-- About -->
<section class="about" id="about">
    <h2>🌸 Our Japanese Story</h2>
    <p>
        Welcome to Sakura Bloom Cafe! Inspired by the beauty
        of Japanese cherry blossoms, we bring you delicious
        matcha drinks, traditional Japanese desserts and
        a peaceful atmosphere. Enjoy every moment with us.
    </p>
</section>

<!-- Menu -->
<section class="menu" id="menu">
    <h2>Our Special Menu</h2>
    <p>Taste the magic of Japan!</p>

    <div class="products">

        <div class="card">
            <img src="https://images.unsplash.com/photo-1515823064-d6e0c04616a7?w=500"
            alt="Matcha Latte">
            <h3>Matcha Latte</h3>
            <p>Fresh Japanese green tea with creamy milk.</p>
            <div class="price">₹180</div>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?w=500"
            alt="Strawberry Cake">
            <h3>Sakura Cake</h3>
            <p>Soft and delicious pink blossom cake.</p>
            <div class="price">₹220</div>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1563805042-7684c019e1cb?w=500"
            alt="Japanese Ice Cream">
            <h3>Mochi Ice Cream</h3>
            <p>Sweet Japanese rice cake with ice cream.</p>
            <div class="price">₹150</div>
        </div>

        <div class="card">
            <img src="https://images.unsplash.com/photo-1551024506-0bccd828d307?w=500"
            alt="Donuts">
            <h3>Sakura Donuts</h3>
            <p>Soft donuts with beautiful pink frosting.</p>
            <div class="price">₹120</div>
        </div>

    </div>
</section>

<!-- Special Offer -->
<section class="special">
    <h2>🌸 Cherry Blossom Special</h2>
    <p>Enjoy our special Sakura combo at just ₹299!</p>
    <br>
    <a href="#contact" class="btn">Visit Us Today</a>
</section>

<!-- Footer -->
<footer id="contact">
    <div class="footer-content">

        <div>
            <h3>Sakura Bloom Cafe</h3>
            <p>A little taste of Japan in every bite.</p>
        </div>

        <div>
            <h3>Opening Hours</h3>
            <p>Monday - Saturday</p>
            <p>9:00 AM - 9:00 PM</p>
        </div>

        <div>
            <h3>Contact Us</h3>
            <p>Email: sakuracafe@gmail.com</p>
            <p>Phone: +91 98765 43210</p>
        </div>

    </div>

    <div class="copyright">
        <p>© 2026 Sakura Bloom Cafe | Made with 🌸 Love</p>
    </div
    ```
</footer>

</body>
</html>


## OUTPUT
![alt text](<output 1.png>)
![alt text](<output 3.png>)
![alt text](<output 2.png>)

## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.