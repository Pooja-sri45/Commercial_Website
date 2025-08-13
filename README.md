# Ex02 Commercial Website
## Date:13/08/2025

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
index.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Elegant Accessories</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <h1>Elegant Accessories</h1>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#products">Our Collection</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>
    
    <section id="home" class="hero">
        <div class="hero-text">
            <img src="mall.jpeg" alt="jewel shop">
            <h1>Graceful Adornments</h1>
            <p>"More than accessories.It’s your signature elegance."</p>
            <a href="#products" class="btn">Buy Now</a>
        </div>
    </section>

    <section id="about" class="about">
        <h2>About Us</h2>
        <p>At Elegant Accessories, we bring you a curated selection of jewellery, handbags, sunglasses, and watches — each crafted with style and sophistication to elevate your everyday look.</p>
    </section>

    <section id="products" class="products">
        <h2>Our Collection</h2>

        <h3>Jewellery</h3>
        <div class="product-container">
            <div class="product">
                <img src="necklace.jpg" alt="Necklace">
                <h4>Diamond Pendant Necklace</h4>
                <p>$1,960</p>

            </div>
            <div class="product">
                <img src="earings.jpg" alt="Earrings">
                <h4>Pearl Drop Earrings</h4>
                <p>$375</p>
            </div>
            <div class="product">
                <img src="bracelet.jpg" alt="Bracelet">
                <h4>Gold Charm Bracelet</h4>
                <p>$560</p>
            </div>
        </div>

        <h3>Fashion Bags</h3>
        <div class="product-container">
            <div class="product">
                <img src="handbag.jpg" alt="Handbag">
                <h4>Leather Tote Bag</h4>
                <p>$280</p>
            </div>
            <div class="product">
                <img src="bag.jpg" alt="Backpack">
                <h4>Designer Backpack</h4>
                <p>$580</p>
            </div>
            <div class="product">
                <img src="clutch.jpg" alt="Clutch">
                <h4>Elegant Evening Clutch</h4>
                <p>$150</p>
            </div>
            
        </div>

        <h3>Sunglasses & Watches</h3>
        <div class="product-container">
            <div class="product">
                <img src="https://images.unsplash.com/photo-1523170335258-f5ed11844a49?w=500" alt="Watch">
                <h4>Minimalist Wrist Watch</h4>
                <p>$410</p>
            </div>
            <div class="product">
                <img src="glasses.jpg" alt="Sunglasses">
                <h4>Classic Aviator Sunglasses</h4>
                <p>$300</p>
            </div>
            <div class="product">
                <img src="watch.jpg" alt="Luxury Watch">
                <h4>Luxury Chronograph Watch</h4>
                <p>$2,000</p>
            </div>
        </div>
    </section>

    <section id="contact" class="contact">
        <h2>Contact Us</h2>
        <p>Email: elegantaccessories@gmail.com</p>
        <p>Phone: +91 9876543210</p>
    </section>

    <footer>
        <p>&copy; 2025 Elegant Accessories | All Rights Reserved</p>
    </footer>
</body>
</html>
```
style.css
```
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body {
  background-color: #fdfdfd;
  color:black
  font-family: 'Open Sans', sans-serif;
  line-height: 1.6;
  font: size 18px;
}
h1, h2, h3 {
  font-family: 'Playfair Display', serif;
  color: black;
}

/* === NAVIGATION === */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 1em 2em;
  background-color: rgb(208, 176, 94);
}
.logo {
  font-size: 1.5em;
  font-weight: bold;
}
.nav-links {
  display: flex;
  gap: 1.5em;
  list-style: none;
}
.nav-links a {
  color: #fff;
  text-decoration: none;
  transition: color 0.3s;
}
.nav-links a:hover {
  color: #121212;
}

/* Header */
header {
    background: #c95db3;
    color: white;
    padding: 15px 20px;
    text-align: center;
    border-radius: 10px;
}

header h1 {
    font-family: 'Playfair Display', serif;
    margin: 0;
}

nav a {
    color: white;
    margin: 0 10px;
    text-decoration: none;
    font-weight: bold;
}

nav a:hover {
    text-decoration: underline;
}

/* Sections */
section {
    padding: 20px;
    text-align: center;
}

section h2 {
    font-family: 'Playfair Display', serif;
    color: #975dc9;
}

section h3 {
    margin-top: 30px;
    color: #3c838b;
}
section h4 {
    margin-top: 20px;
    color: black;
}

/* === HERO === */
.hero {
  min-height: 90vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
}
.hero img {
  max-width: 100%;
  border-radius: 8px;
}
.hero-text {
  animation: fadeIn 2s ease-in;
}
.hero h1 {
  font-size: 3em;
}
.btn {
  background: goldenrod;
  color: #121212;
  padding: 0.7em 1.5em;
  border-radius: 5px;
  text-decoration: none;
  transition: all 0.3s;
  display: inline-block;
  margin-top: 1em;
}
.btn:hover {
  background: linear-gradient(45deg, goldenrod, silver);
}
/* === ABOUT === */
.about {
  padding: 3em 2em;
  text-align: center;
  font-size: 18px; 
}
/* Product Cards */
.product-container {
    display: flex;
    justify-content: center;
    gap: 20px;
    flex-wrap: wrap;
    margin-bottom: 30px;
}

.product {
    background: #fff;
    padding: 10px;
    border: 2px solid #c97c5d;
    border-radius: 12px;
    width: 180px;
    text-align: center;
    box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    transition: transform 0.3s, box-shadow 0.3s;
}

.product img {
    width: 100%;
    border-radius: 10px;
}

.product:hover {
    transform: translateY(-5px);
    box-shadow: 0 8px 16px rgba(0,0,0,0.2);
}

/* Footer */
footer {
    background-color: #222;
    text-align: center;
    padding: 1em;
    color: white;
}
```

## OUTPUT
<img width="1919" height="1079" alt="Screenshot 2025-08-13 192019" src="https://github.com/user-attachments/assets/9babfdf2-9b9b-4dba-a924-78c5e9634c03" />
<img width="1919" height="1079" alt="Screenshot 2025-08-13 192046" src="https://github.com/user-attachments/assets/5c0ba601-6404-44db-9ad4-2708263f3950" />
<img width="1919" height="1079" alt="Screenshot 2025-08-13 192008" src="https://github.com/user-attachments/assets/42e14fe8-8905-4b39-b300-befddbdfe284" />




## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
