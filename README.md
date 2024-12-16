# Ex.07 Restaurant Website
## Date:16.12.2024

## AIM:
To develop a static Restaurant website to display the food items and services provided by them.

## DESIGN STEPS:

### Step 1:
Requirement collection.

### Step 2:
Creating the layout using HTML and CSS.

### Step 3:
Updating the sample content.

### Step 4:
Choose the appropriate style and color scheme.

### Step 5:
Validate the layout in various browsers.

### Step 6:
Validate the HTML code.

### Step 7:
Publish the website in the given URL.

## PROGRAM:
'''
index.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SP Spicy Restaurant - Italian Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">SP Spicy Restaurant</div>
            <ul>
                <li><a href="index.html" class="active">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="admin.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <main>
        <section class="hero">
            <div class="hero-content">
                <h1>Welcome to SP SPICY RESTAURANT</h1>
                <p>Experience authentic Italian cuisine in a warm and elegant atmosphere</p>
                <a href="menu.html" class="cta-button">View Our Menu</a>
            </div>
        </section>

        <section class="features">
            <div class="feature">
                <h2>Traditional Recipes</h2>
                <p>Passed down through generations</p>
            </div>
            <div class="feature">
                <h2>Fresh Ingredients</h2>
                <p>Locally sourced and organic</p>
            </div>
            <div class="feature">
                <h2>Expert Chefs</h2>
                <p>Trained in Italy's finest kitchens</p>
            </div>
        </section>
    </main>

    <footer>
        <p>© 2024 SP Spicy Restaurant. Designed by [NAVEEN KUMAR]</p>
    </footer>

</body>
</html>

style.css

/* Base styles */
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: 'Helvetica Neue', Arial, sans-serif;
    line-height: 1.6;
    color: #333333;
    background-color: #FFF8DC;
}

/* Header and Navigation */
header {
    background-color: #8B4513;
    padding: 1rem;
    position: fixed;
    width: 100%;
    top: 0;
    z-index: 1000;
}

nav {
    max-width: 1200px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    color: #FFF8DC;
    font-size: 1.5rem;
    font-weight: bold;
}

nav ul {
    display: flex;
    list-style: none;
}

nav ul li a {
    color: #FFF8DC;
    text-decoration: none;
    padding: 0.5rem 1rem;
    margin: 0 0.5rem;
    border-radius: 4px;
    transition: background-color 0.3s;
}

nav ul li a:hover,
nav ul li a.active {
    background-color: #CD853F;
}

/* Main Content */
main {
    margin-top: 80px;
    padding: 2rem;
    max-width: 1200px;
    margin-left: auto;
    margin-right: auto;
}

/* Hero Section */
.hero {
    background-image: url('Inside.jpeg');
    background-size: cover;
    background-position: center;
    height: 600px;
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    color: #FFF8DC;
    margin: -2rem -2rem 2rem -2rem;
}

.hero-content {
    background-color: rgba(139, 69, 19, 0.8);
    padding: 2rem;
    border-radius: 8px;
}

.hero h1 {
    font-size: 3rem;
    margin-bottom: 1rem;
}

.cta-button {
    display: inline-block;
    background-color: #CD853F;
    color: #FFF8DC;
    padding: 1rem 2rem;
    border-radius: 4px;
    text-decoration: none;
    margin-top: 1rem;
    transition: background-color 0.3s;
}

.cta-button:hover {
    background-color: #8B4513;
}

/* Features Section */
.features {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 2rem;
    margin-top: 3rem;
}

.feature {
    text-align: center;
    padding: 2rem;
    background-color: #fff;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

/* Menu Page */
.menu-section {
    margin-bottom: 3rem;
}

.menu-section h2 {
    color: #8B4513;
    margin-bottom: 1.5rem;
}

.menu-items {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 1.5rem;
}

.menu-item {
    background-color: #fff;
    padding: 1.5rem;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.menu-item h3 {
    color: #8B4513;
    margin-bottom: 0.5rem;
}

.price {
    color: #CD853F;
    font-weight: bold;
    font-size: 1.2rem;
}

/* Administration Page */
.team-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 2rem;
    margin-top: 2rem;
}

.team-member {
    background-color: #fff;
    padding: 1.5rem;
    border-radius: 8px;
    text-align: center;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.team-member img {
    width: 200px;
    height: 200px;
    border-radius: 50%;
    margin-bottom: 1rem;
    object-fit: cover;
}

/* Contact Page */
.contact-container {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
    margin-top: 2rem;
}

.contact-info,
.contact-form {
    background-color: #fff;
    padding: 2rem;
    border-radius: 8px;
    box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.form-group {
    margin-bottom: 1rem;
}

label {
    display: block;
    margin-bottom: 0.5rem;
}

input,
textarea {
    width: 100%;
    padding: 0.5rem;
    border: 1px solid #ddd;
    border-radius: 4px;
}

textarea {
    height: 150px;
}

button {
    background-color: #8B4513;
    color: #FFF8DC;
    padding: 0.5rem 1rem;
    border: none;
    border-radius: 4px;
    cursor: pointer;
    transition: background-color 0.3s;
}

button:hover {
    background-color: #CD853F;
}

/* Footer */
footer {
    background-color: #8B4513;
    color: #FFF8DC;
    text-align: center;
    padding: 1rem;
    margin-top: 2rem;
}


@media (max-width: 768px) {
    nav {
        flex-direction: column;
        text-align: center;
    }

    nav ul {
        margin-top: 1rem;
        flex-wrap: wrap;
        justify-content: center;
    }

    .features {
        grid-template-columns: 1fr;
    }

    .contact-container {
        grid-template-columns: 1fr;
    }

    .hero h1 {
        font-size: 2rem;
    }
}

admin.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Administration - SP spicy Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">SP Spicy Restaurant</div>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="admin.html" class="active">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <main class="admin-page">
        <h1>Our Team</h1>
        
        <div class="team-grid">
            <div class="team-member">
                <img src="OIP.jpeg" alt="Marco Rossi">
                <h3>Marco Rossi</h3>
                <p>Executive Chef</p>
            </div>
            <div class="team-member">
                <img src="portrait.avif" alt="Sofia Bianchi">
                <h3>Sofia Bianchi</h3>
                <p>Restaurant Manager</p>
            </div>
            <div class="team-member">
                <img src="depositphotos.jpg" alt="Luca Conti">
                <h3>Luca Conti</h3>
                <p>Sous Chef</p>
            </div>
            <div class="team-member">
                <img src="104-Pastry.jpg" alt="Isabella Romano">
                <h3>Isabella Romano</h3>
                <p>Pastry Chef</p>
            </div>
            <div class="team-member">
                <img src="Restaurant-chefs.jpg" alt="Giuseppe Marino">
                <h3>Giuseppe Marino</h3>
                <p>Head Sommelier</p>
            </div>
            <div class="team-member">
                <img src="OIP (1).jpeg" alt="Elena Ferrari">
                <h3>Elena Ferrari</h3>
                <p>Events Coordinator</p>
            </div>
        </div>
    </main>

    <footer>
        <p>© 2024 SP Spicy Restaurant. Designed by [NAVEEN KUMAR]</p>
    </footer>
</body>
</html>


contuct.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us - SP Spicy Restaurant</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">SP Spicy Restaurant</div>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="menu.html">Menu</a></li>
                <li><a href="admin.html">Administration</a></li>
                <li><a href="contact.html" class="active">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <main class="contact-page">
        <h1>Contact Us</h1>
        
        <div class="contact-container">
            <div class="contact-info">
                <h2>Visit Us</h2>
                <address>
                    <p>123 Italian Street</p>
                    <p>Cuisine District</p>
                    <p>New York, NY 10001</p>
                </address>

                <h2>Contact Information</h2>
                <p>Phone: 93335-93335</p>
                <p>Email: infospspicyrest@gmail.com</p>

                <h2>Hours of Operation</h2>
                <p>Monday - Thursday: 11:30 AM - 10:00 PM</p>
                <p>Friday - Saturday: 11:30 AM - 11:00 PM</p>
                <p>Sunday: 12:00 PM - 9:00 PM</p>
            </div>

            <div class="contact-form">
                <h2>Send us a Message</h2>
                <form>
                    <div class="form-group">
                        <label for="name">Name:</label>
                        <input type="text" id="name" name="name" required>
                    </div>
                    <div class="form-group">
                        <label for="email">Email:</label>
                        <input type="email" id="email" name="email" required>
                    </div>
                    <div class="form-group">
                        <label for="message">Message:</label>
                        <textarea id="message" name="message" required></textarea>
                    </div>
                    <button type="submit">Send Message</button>
                </form>
            </div>
        </div>
    </main>

    <footer>
        <p>© 2024 SP Spicy Restaurant. Designed by [NAVEEN KUMAR]</p>
    </footer>
</body>
</html>


menu.html


<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Menu - La Bella Cucina</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header>
        <nav>
            <div class="logo">SP Spicy Restaurant</div>
            <ul>
                <li><a href="index.html">Home</a></li>
                <li><a href="menu.html" class="active">Menu</a></li>
                <li><a href="admin.html">Administration</a></li>
                <li><a href="contact.html">Contact Us</a></li>
            </ul>
        </nav>
    </header>

    <main class="menu-page">
        <h1>Our Menu</h1>
        
        <section class="menu-section">
            <h2>Appetizers</h2>
            <div class="menu-items">
                <div class="menu-item">
                    <h3>Bruschetta</h3>
                    <p>Toasted bread with fresh tomatoes, garlic, and basil</p>
                    <span class="price">$8</span>
                </div>
                <div class="menu-item">
                    <h3>Caprese Salad</h3>
                    <p>Fresh mozzarella, tomatoes, and basil with balsamic glaze</p>
                    <span class="price">$10</span>
                </div>
                <div class="menu-item">
                    <h3>Calamari Fritti</h3>
                    <p>Crispy fried calamari with marinara sauce</p>
                    <span class="price">$12</span>
                </div>
            </div>
        </section>

        <section class="menu-section">
            <h2>Pasta</h2>
            <div class="menu-items">
                <div class="menu-item">
                    <h3>Spaghetti Carbonara</h3>
                    <p>Classic carbonara with pancetta and pecorino</p>
                    <span class="price">$16</span>
                </div>
                <div class="menu-item">
                    <h3>Fettuccine Alfredo</h3>
                    <p>Creamy parmesan sauce with fresh pasta</p>
                    <span class="price">$15</span>
                </div>
                <div class="menu-item">
                    <h3>Penne Arrabbiata</h3>
                    <p>Spicy tomato sauce with garlic and herbs</p>
                    <span class="price">$14</span>
                </div>
            </div>
        </section>

        <section class="menu-section">
            <h2>Main Courses</h2>
            <div class="menu-items">
                <div class="menu-item">
                    <h3>Osso Buco</h3>
                    <p>Braised veal shanks with gremolata</p>
                    <span class="price">$28</span>
                </div>
                <div class="menu-item">
                    <h3>Chicken Marsala</h3>
                    <p>Pan-seared chicken with mushroom marsala sauce</p>
                    <span class="price">$24</span>
                </div>
                <div class="menu-item">
                    <h3>Grilled Sea Bass</h3>
                    <p>Fresh sea bass with lemon herb sauce</p>
                    <span class="price">$32</span>
                </div>
            </div>
        </section>

        <section class="menu-section">
            <h2>Desserts</h2>
            <div class="menu-items">
                <div class="menu-item">
                    <h3>Tiramisu</h3>
                    <p>Classic Italian coffee-flavored dessert</p>
                    <span class="price">$8</span>
                </div>
                <div class="menu-item">
                    <h3>Panna Cotta</h3>
                    <p>Vanilla cream with berry compote</p>
                    <span class="price">$7</span>
                </div>
                <div class="menu-item">
                    <h3>Cannoli</h3>
                    <p>Sicilian pastry filled with sweet ricotta</p>
                    <span class="price">$6</span>
                </div>
            </div>
        </section>
    </main>

    <footer>
        <p>© 2024 SP Spicy Restaurant. Designed by [NAVEEN KUMAR]</p>
    </footer>
</body>
</html>



'''


## OUTPUT:

![alt text](<rest/Screenshot 2024-12-16 203158.png>)
![alt text](<rest/Screenshot 2024-12-16 203229.png>)
![alt text](<rest/Screenshot 2024-12-16 203257.png>)
![alt text](<rest/Screenshot 2024-12-16 203310.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
