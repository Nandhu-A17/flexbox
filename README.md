# flexbox
# Ex02 Commercial Website
# Date: 31-10-2026
# AIM
To create a commercial website using CSS Flexbox.

# ALGORITHM

STEP 1

Create an HTML file (index.html)

STEP 2

Create a CSS file (style.css)

STEP 3

Include a navigation bar with links to different sections.

STEP 4

Add structured sections for Homepage, Products / Services, About Us, Contact Details and User Account.

STEP 5

Include social media links at the footer with copyright information.

STEP 6

Define global styles for fonts, colors, and layout.

STEP 7

Style the header, navigation bar, and sections.

STEP 8

Use Flexbox for layout design.

STEP 9

Add hover effects and transitions for interactivity.

STEP 10

Add Images and Media.

STEP 11

Use optimized images for a professional look.

STEP 12

Open the HTML file in a browser to check layout and functionality.

STEP 13

Fix styling issues and refine content placement.

STEP 14

Deploy the website.

STEP 15

Upload to GitHub Pages for free hosting.

# PROGRAM
## index.html 

```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Bloom & Bliss | Flower Boutique</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>

    <!-- Navigation Bar -->
    <header>
        <div class="logo">🌸 Bloom & Bliss</div>

        <nav>
            <a href="#">Home</a>
            <a href="#flowers">Flowers</a>
            <a href="#about">About</a>
            <a href="#contact">Contact</a>
        </nav>

        <a href="#flowers" class="nav-btn">Shop Now</a>
    </header>

    <!-- Hero Section -->
    <section class="hero">

        <div class="hero-content">
            <p class="tagline">FRESH FLOWERS • HAPPY MOMENTS</p>

            <h1>
                Say It With<br>
                <span>Beautiful Flowers.</span>
            </h1>

            <p class="description">
                Make every moment special with our fresh and
                beautiful flowers, carefully arranged with love.
            </p>

            <a href="#flowers" class="primary-btn">Explore Flowers →</a>
        </div>

        <div class="hero-image">
            <img src="Title image.avif"
                 alt="Beautiful Flower Bouquet">
        </div>

    </section>

    <!-- Features Section -->
    <section class="features">

        <div class="feature">
            <span>🌷</span>
            <h3>Fresh Flowers</h3>
            <p>Freshly picked every day</p>
        </div>

        <div class="feature">
            <span>🎁</span>
            <h3>Beautiful Gifts</h3>
            <p>Perfect for every occasion</p>
        </div>

        <div class="feature">
            <span>🚚</span>
            <h3>Fast Delivery</h3>
            <p>Flowers delivered with care</p>
        </div>

    </section>

    <!-- Flower Products -->
    <section class="flowers" id="flowers">

        <div class="section-heading">
            <p>OUR COLLECTION</p>
            <h2>Flowers That Speak Love</h2>
            <span>Choose your favorite bouquet.</span>
        </div>

        <div class="flower-container">

            <div class="flower-card">
                <img src="img2.avif"
                     alt="Rose Bouquet">

                <div class="card-content">
                    <h3>Classic Rose Bouquet</h3>
                    <p>Romantic red roses for your loved ones.</p>

                    <div class="price">
                        <h4>₹599</h4>
                        <button>+</button>
                    </div>
                </div>
            </div>

            <div class="flower-card">
                <img src="img3.avif"
                     alt="Pink Flowers">

                <div class="card-content">
                    <h3>Pink Blossom</h3>
                    <p>Soft pink flowers for sweet moments.</p>

                    <div class="price">
                        <h4>₹799</h4>
                        <button>+</button>
                    </div>
                </div>
            </div>

            <div class="flower-card">
                <img src="img 4.avif"
                     alt="White Flowers">

                <div class="card-content">
                    <h3>Elegant White Bouquet</h3>
                    <p>Beautiful white flowers for every occasion.</p>

                    <div class="price">
                        <h4>₹699</h4>
                        <button>+</button>
                    </div>
                </div>
            </div>

        </div>

    </section>

    <!-- Special Offer -->
    <section class="offer">

        <div class="offer-content">
            <p>SPECIAL OFFER</p>

            <h2>Make Someone<br>Feel Special!</h2>

            <h3>Get 20% OFF on your first flower order.</h3>

            <a href="#flowers" class="offer-btn">Shop Flowers</a>
        </div>

        <div class="offer-image">
            <img src="img1.avif"
                 alt="Flower Special Offer">
        </div>

    </section>

    <!-- About Section -->
    <section class="about" id="about">

        <p>OUR STORY</p>

        <h2>Flowers Make Life Beautiful</h2>

        <p class="about-text">
            At Bloom & Bliss, we believe every flower tells a story.
            Our beautiful floral arrangements are created with love
            and care to make your special moments unforgettable.
            From birthdays to anniversaries, we bring happiness
            through flowers.
        </p>

    </section>

    <!-- Footer -->
    <footer id="contact">

        <h2>🌸 Bloom & Bliss</h2>

        <p>Bringing happiness through flowers.</p>

        <p>Email: bloomandbliss@gmail.com</p>

        <p>© 2026 Bloom & Bliss. All Rights Reserved.</p>

    </footer>

</body>
</html>
```
## style.css

```
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    background-color: #fffaf7;
    color: #4a3038;
}

/* Navigation */

header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 22px 8%;
    background-color: white;
}

.logo {
    font-size: 24px;
    font-weight: bold;
    color: #b34b72;
}

nav {
    display: flex;
    gap: 30px;
}

nav a {
    text-decoration: none;
    color: #4a3038;
    font-size: 14px;
}

nav a:hover {
    color: #c75b83;
}

.nav-btn {
    background-color: #b34b72;
    color: white;
    padding: 12px 22px;
    text-decoration: none;
    border-radius: 25px;
}

/* Hero Section */

.hero {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 70px 8%;
    gap: 50px;
}

.hero-content {
    flex: 1;
}

.tagline {
    color: #b34b72;
    font-size: 12px;
    letter-spacing: 3px;
    font-weight: bold;
    margin-bottom: 20px;
}

.hero h1 {
    font-size: 55px;
    line-height: 1.2;
    margin-bottom: 20px;
}

.hero h1 span {
    color: #c75b83;
}

.description {
    color: #806c72;
    line-height: 1.8;
    margin-bottom: 30px;
    max-width: 450px;
}

.primary-btn {
    display: inline-block;
    background-color: #b34b72;
    color: white;
    padding: 15px 25px;
    text-decoration: none;
    border-radius: 30px;
    transition: 0.3s;
}

.primary-btn:hover {
    background-color: #863650;
}

.hero-image {
    flex: 1;
}

.hero-image img {
    width: 100%;
    height: 430px;
    object-fit: cover;
    border-radius: 45% 45% 15px 15px;
}

/* Features */

.features {
    display: flex;
    justify-content: space-around;
    align-items: center;
    background-color: #f5e4e9;
    padding: 35px 8%;
    text-align: center;
    gap: 20px;
}

.feature span {
    font-size: 30px;
}

.feature h3 {
    margin: 10px 0;
}

.feature p {
    color: #806c72;
    font-size: 13px;
}

/* Flower Products */

.flowers {
    padding: 75px 8%;
}

.section-heading {
    text-align: center;
    margin-bottom: 40px;
}

.section-heading p {
    color: #b34b72;
    font-size: 12px;
    letter-spacing: 3px;
    font-weight: bold;
}

.section-heading h2 {
    font-size: 35px;
    margin: 15px 0;
}

.section-heading span {
    color: #806c72;
}

.flower-container {
    display: flex;
    justify-content: center;
    gap: 30px;
    flex-wrap: wrap;
}

.flower-card {
    background-color: white;
    width: 300px;
    border-radius: 15px;
    overflow: hidden;
    box-shadow: 0 8px 25px rgba(100, 40, 60, 0.10);
    transition: 0.3s;
}

.flower-card:hover {
    transform: translateY(-8px);
}

.flower-card img {
    width: 100%;
    height: 220px;
    object-fit: cover;
}

.card-content {
    padding: 22px;
}

.card-content h3 {
    margin-bottom: 10px;
}

.card-content p {
    color: #806c72;
    font-size: 14px;
}

.price {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-top: 20px;
}

.price h4 {
    color: #b34b72;
    font-size: 20px;
}

.price button {
    background-color: #b34b72;
    color: white;
    border: none;
    width: 35px;
    height: 35px;
    border-radius: 50%;
    font-size: 22px;
    cursor: pointer;
}

/* Offer Section */

.offer {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 40px;
    background-color: #5a3545;
    color: white;
    padding: 60px 8%;
}

.offer-content {
    flex: 1;
}

.offer p {
    color: #f3b7ca;
    letter-spacing: 3px;
    margin-bottom: 15px;
}

.offer h2 {
    font-size: 40px;
    line-height: 1.3;
    margin-bottom: 15px;
}

.offer h3 {
    font-size: 16px;
    font-weight: normal;
    margin-bottom: 25px;
}

.offer-btn {
    display: inline-block;
    background-color: #f3b7ca;
    color: #5a3545;
    padding: 13px 25px;
    border-radius: 25px;
    text-decoration: none;
    font-weight: bold;
}

.offer-image {
    flex: 1;
}

.offer-image img {
    width: 100%;
    height: 300px;
    object-fit: cover;
    border-radius: 15px;
}

/* About */

.about {
    padding: 70px 15%;
    text-align: center;
}

.about > p:first-child {
    color: #b34b72;
    letter-spacing: 3px;
    font-weight: bold;
}

.about h2 {
    font-size: 32px;
    margin: 20px 0;
}

.about-text {
    color: #806c72;
    line-height: 1.8;
}

/* Footer */

footer {
    background-color: #38232d;
    color: white;
    text-align: center;
    padding: 35px;
    line-height: 2;
}

footer h2 {
    color: #f3b7ca;
}

/* Responsive Design */

@media (max-width: 768px) {

    header {
        flex-direction: column;
        gap: 20px;
    }

    nav {
        flex-wrap: wrap;
        justify-content: center;
        gap: 15px;
    }

    .hero {
        flex-direction: column;
        text-align: center;
    }

    .hero h1 {
        font-size: 40px;
    }

    .hero-image img {
        height: 300px;
    }

    .features {
        flex-direction: column;
        gap: 30px;
    }

    .offer {
        flex-direction: column;
        text-align: center;
    }

    .offer h2 {
        font-size: 32px;
    }
}

```

# OUTPUT
![alt text](<output img.png>)

![alt text](<output img2.png>)

![alt text](<output img3.png>)

# RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.

