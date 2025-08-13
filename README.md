# Ex02 Commercial Website
## Date: 13.08.2025

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
## HTML:
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Multiplex Signs | Chennai Signboard Experts</title>
    <link rel="stylesheet" href="05.css">
</head>
<body>

    <!-- HEADER -->
    <header>
        <div class="logo-title">
            <img src="logo1.png" alt="Multiplex Signs Logo" class="logo-img">
            <span class="site-title">Multiplex Signs</span>
        </div>
        <nav>
            <a href="#home">Home</a>
            <a href="#services">Our Services</a>
            <a href="#about">About Us</a>
            <a href="#clients">Clients</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <!-- HERO / HOME SECTION -->
    <section id="home" class="hero">
        <div class="hero-content">
            <h1>Creating Eye-Catching Signboards for Every Business</h1>
            <p>Multiplex established in 2000. Chennai's trusted experts for all kinds of signage—quality, creativity, competitive rates, own designing and fabrication units.</p>
            <a href="#contact" class="btn">Get A Free Quote</a>
        </div>
    </section>

    <!-- Services Section -->
    <section id="services" class="services">
        <h2>Our Services</h2>
        <div class="card-container">
            <div class="card led-board">
                <h3>LED Boards</h3>
                <p>Bright and durable boards for high visibility.</p>
            </div>
            <div class="card acp-board">
                <h3>ACP Boards</h3>
                <p>Modern Aluminum Composite Panels for signage.</p>
            </div>
            <div class="card letters-board">
                <h3>Letters</h3>
                <p>Custom cut acrylic and metal letters for branding.</p>
            </div>
            <div class="card glow-board">
                <h3>Glow Signage</h3>
                <p>Illuminated boards that shine night and day!</p>
            </div>
            <div class="card nonlit-board">
                <h3>Non Lit Signage</h3>
                <p>Elegant boards for indoor & outdoor use.</p>
            </div>
        </div>
    </section>

    <!-- Clients Section -->
    <section id="clients" class="clients">
        <h2>Our Clients</h2>
        <div class="card-container">
            <div class="card client1-board">
                
            </div>
            <div class="card client2-board">
                
            </div>
            <div class="card client3-board">
                
            </div>
            <div class="card client4-board">
                
            </div>
        </div>
    </section>
    
    <!-- About Us Section -->
    <section id="about" class="order">
        <h2>About Us</h2>
        <p>
            Multiplex established in 2000 and we do all kinds of signage.<br>
            We have our own Designing Unit, Fabrication Unit, Machineries.<br>
            We do our best quality and competitive rates.
        </p>
        <ul>
            <li>Own designing & fabrication units</li>
            <li>Expert team & advanced equipment</li>
            <li>Trusted by Chennai's leading brands</li>
        </ul>
    </section>
    
    <!-- Contact Section -->
    <section id="contact" class="menu">
        <h2>Contact Us</h2>
        <div class="branches">
            <div class="branch">
                <h3>Mount Road</h3>
                <p>New No.27, Old No.14, Thayar Sahib Street,<br>
                Chennai – 600 002.<br>
                (1st Left of G.P. Road) (Near Ellis Road)</p>
            </div>
            <div class="branch">
                <h3>Iyyappanthangal</h3>
                <p>No. 81, Mount Poonamallee Road,<br>
                Iyyappanthangal, Chennai – 600 056.<br>
                (Opp To Porur Sri Ramachandra Hospital)</p>
            </div>
        </div>
        <div class="contact-details">
            <div>
                <strong>📞 Phone:</strong> 9840084893, 9841684803
            </div>
            <div>
                <strong>📧 Email:</strong> <a href="mailto:multiplexsignage@yahoo.com">multiplexsignage@yahoo.com</a>
            </div>
            <div>
                <strong>💳 GPay:</strong> MULTIPLEX (9841684893@okbizaxis)
            </div>
        </div>
    </section>
    
    <!-- Footer -->
    <footer>
        <p>© 2025 Multiplex Signs | All Rights Reserved</p>
        <p>Designed by AshwinKumar A</p>
        <div class="social-links">
            <a href="https://multiplexsigns.com/index.html">Facebook</a> | 
            <a href="https://multiplexsigns.com/index.html">Instagram</a> | 
            <a href="https://api.whatsapp.com/send?phone=919840084893">WhatsApp</a>
        </div>
    </footer>
</body>
</html>
```
## CSS:
```css
/* ===== General Reset ===== */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
}

/* ===== Header ===== */
header {
    background: #222;
    color: white;
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 12px 20px;
}
header .logo-title {
    display: flex;
    align-items: center;
}
header .logo-img {
    height: 50px;
    margin-right: 10px;
}
header nav a {
    color: white;
    text-decoration: none;
    margin-left: 20px;
}
header nav a:hover {
    text-decoration: underline;
}
.site-title {
    color: #FFF7B2;
    font-family: 'Poppins', Arial, sans-serif;
    font-size: 2rem;
    font-weight: 600;
}
/* ===== Hero Section ===== */
.hero {
    background: url('banner.png') center/cover no-repeat;
    color: white;
    text-align: center;
    padding: 80px 20px;
}
.hero h1 {
    font-size: 2.2em;
}
.hero p {
    max-width: 700px;
    margin: 10px auto 20px;
}
.btn {
    background: orange;
    color: white;
    padding: 10px 20px;
    text-decoration: none;
    font-weight: bold;
    border-radius: 5px;
}
.btn:hover {
    background: darkorange;
}

section {
  padding: 40px 0;
  text-align: center;
}

section h2 {
  font-size: 2rem;
  color: #2b3a4a;
  margin-bottom: 30px;
}

.card-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 20px;
}

.card {
  background-color: #fdf9e8;
  border-radius: 12px;
  box-shadow: 0 4px 10px rgba(0,0,0,0.1);
  padding: 20px;
  width: 180px;
  text-align: center;
  transition: transform 0.2s ease;
}

.card:hover {
  transform: translateY(-5px);
}

.card img {
  width: 50px;
  height: 50px;
  object-fit: contain;
  margin-bottom: 10px;
}

.card.led-board {
    background: url('led.jpg') center/cover no-repeat, #fdf9e8;
}
.card.acp-board {
    background: url('acp.jpg') center/cover no-repeat, #fdf9e8;
}
.card.letters-board {
    background: url('letter.jpg') center/cover no-repeat, #fdf9e8;
}
.card.glow-board {
    background: url('gs.jpg') center/cover no-repeat, #fdf9e8;
}
.card.nonlit-board {
    background: url('nls.jpg') center/cover no-repeat, #fdf9e8;
}

/* Clients */
.card.client1-board {
    background: url('client1.png') center/cover no-repeat, #fdf9e8;
}
.card.client2-board {
    background: url('client2.png') center/cover no-repeat, #fdf9e8;
}
.card.client3-board {
    background: url('client3.png') center/cover no-repeat, #fdf9e8;
}
.card.client4-board {
    background: url('client4.png') center/cover no-repeat, #fdf9e8;
}
/* ...repeat for other card types... */
/* Optionally, add a semi-transparent overlay for text readability */
.card h3, .card p {
    background: rgba(255,255,255,0.7);
    display: inline-block;
    padding: 4px 8px;
    border-radius: 6px;
    margin-bottom: 6px;
}

/* ===== About Us ===== */
.order {
    padding: 40px 20px;
    background: #fffde9; /* softer yellow */
    text-align: center;
}
.order h2 {
    font-family: 'Poppins', Arial, sans-serif;
    font-size: 2rem;
    font-weight: bold;
    color: #2b3a4a;
    margin-bottom: 18px;
}
.order p {
    font-size: 1.1rem;
    color: #222;
    margin-bottom: 18px;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    line-height: 1.5;
}
.order ul {
    display: inline-block;
    text-align: left;
    margin-top: 10px;
    padding-left: 24px;
}
.order li {
    margin-bottom: 8px;
    font-size: 1.05rem;
    color: #222;
}
.order ul {
    margin-top: 10px;
    padding-left: 20px;
}
.order li {
    margin-bottom: 8px;
}

/* Contact Section */
.menu#contact {
    background: #f8f6ec;
    padding-bottom: 19px;
}
.branches {
    display: flex;
    gap: 18px;
    justify-content: center;
    flex-wrap: wrap;
    margin-bottom: 24px;
}
.branch {
    background: #fff9d7;
    border-radius: 10px;
    padding: 13px 20px;
    min-width: 250px;
    box-shadow: 0 1px 4px #ffe18652;
}
.branch h3 {
    color: #a68900;
    margin-bottom: 3px;
}
.contact-details {
    display: flex;
    gap: 19px;
    justify-content: center;
    flex-wrap: wrap;
    margin-bottom: 8px;
}
.contact-details div {
    background: #fff8e1;
    padding: 10px 18px;
    border-radius: 8px;
    min-width: 160px;
    font-size: 1.01em;
}
.contact-details a {
    color: #36415a;
    text-decoration: underline;
}

/* Footer */
footer {
    background-color: #36415a;
    color: white;
    text-align: center;
    padding: 24px 10px;
    line-height: 1.7;
    font-family: 'Poppins', Arial, sans-serif;
}
footer p {
    margin: 6px 0;
}
.social-links a {
    color: #FFD700;
    text-decoration: none;
    font-weight: 500;
    margin: 0 4px;
}
.social-links a:hover {
    color: #fff;
    text-decoration: underline;
}

/* Responsive Styles */
@media (max-width: 820px) {
    .branches, .menu-grid, .specials-grid, .contact-details {
        flex-direction: column;
        align-items: center;
        gap: 15px;
    }
    .navbar {
        flex-direction: column;
        gap: 10px;
        padding: 22px 2vw;
    }
}
@media (max-width: 510px) {
    .hero-text h1 { font-size: 1.4rem; }
    .card { width: 88vw; }
    .branch { min-width: 70vw; }
}
```

## OUTPUT

<img width="1919" height="1030" alt="image" src="https://github.com/user-attachments/assets/4f1a2639-b491-41c1-972b-205fac1baaf7" />

<img width="1919" height="1029" alt="image" src="https://github.com/user-attachments/assets/2e23109d-8ee4-434c-8451-eea4b392de90" />

<img width="1919" height="1032" alt="image" src="https://github.com/user-attachments/assets/c57a92d2-af37-492d-ba63-81e9da07cbbb" />




## RESULT
The program for creating commercial website using CSS Flexbox is executed successfully.
