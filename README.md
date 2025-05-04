# Ex.07 Restaurant Website
## Date:04.05.2025

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
```
<html>
<head>
    <title>Delicious Bites</title>
    <style>
      
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: white;
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;
            
        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }

        .banner {
            background-size: cover;
            margin-right: 2%;
            margin-left: 2%;
            margin-top: 1%;
            border-radius: 37px;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 30px 20px;
            background: url('banner.jpg') no-repeat center center/cover;
            color: white;
            height: 300px;
            text-align: center;
            background-image: url(bg1.jpeg);
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size: cover;
        }

        .banner-content {
            max-width: 50%;
        }

        .banner-content h1 {
            font-family: Georgia, 'Times New Roman', Times, serif;
            font-size: 2.5rem;
            margin-bottom: 10px;
            color: rgb(175, 175, 175);
        }

        .banner-content p {
            font-size: 1rem;
            margin-bottom: 15px;
            color: rgb(175, 175, 175);
        }

        .banner-content a {
            background: transparent;
            color: rgb(175, 175, 175);
            padding: 8px 15px;
            text-decoration: none;
            font-weight: bold;
            border-radius: 5px;
            border: solid;
            border-color: #676767;
            transition: background 0.3s ease;
        }

        .banner-content a:hover {
            background: #ffffff;
        }

        .features {
            display: flex  ;
            justify-content: space-between;
            align-items: flex-start;
            padding: 20px;
            gap: 15px;
            background: #f9f9f9;
            background-image: url(bg2.jpg);
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size: cover;
        }

        .feature {
            background: white;
            border-radius: 10px;
            padding: 15px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            flex: 1;
            text-align: center;
        }

        .feature img {
            width: 100%;
            border-radius: 10px;
            margin-bottom: 10px;
        }

        .feature h3 {
            font-size: 1.2rem;
            margin-bottom: 10px;
            color: #1f1714;
        }

        .feature p {
            font-size: 0.9rem;
            color: #555;
        }

        footer {
            background: rgb(4, 186, 95);
            color: rgb(0, 0, 0);
            text-align: center;
            padding: px 0;
            margin-top: 180px;
        }


        @media (max-width: 768px) {
            .banner {
                flex-direction: column;
                height: auto;
                text-align: center;
            }

            .banner-content {
                max-width: 100%;
            }

            .features {
                flex-direction: column;
                gap: 20px;
            }

            .feature {
                flex: none;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="1logo.webp" href="home.html" alt="Delicious Bites Logo">
            <div class="ltext "><h1 >Delicious Bites</h1></div>
        </div>
        
            <nav>
                <a href="home.html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>
    <hr width="95%"> 
    <div class="banner">
        <div class="banner-content">
            <h1>Welcome to Delicious Bites</h1>
            <p>Your destination for mouth-watering dishes....</p>
            <a href="#features">Explore Now</a>
        </div>
    </div>

    <section id="features" class="features">
        <div class="feature">
            <img src="candlelight.jpeg" alt="Candle Light Dinner">
            <h3>Candle Light Dinner</h3>
            <p> Candlelight has a timeless charm that creates the perfect backdrop for love 
            to blossom.The enduring companionship of candlelight and romance has woven countless
             enchanting tales through the ages.</p>
        </div>
        <div class="feature">
            <img src="ambience.jpeg" alt="Unique Ambiance">
            <h3>Unique Ambiance</h3>
            <p>Immerse yourself in a cozy ambiance, complete with elegant nautical decor.Once
             You come to our reataurent, you will neverforget the taste.Come and Enjoy with Family.</p>
        </div>
        <div class="feature">
            <img src="1Kaara Azhagar.webp" alt="Iconic Dishes">
            <h3>Iconic Dish</h3>
            <p>Kaara Azhagar is a traditional Tamil dish that combines roasted lentils and spices with tamarind,
               creating a tangy and spicy curry. Unlike regular sambars or kuzhambus, Kaara Azhagar stands out.</p>
        </div>
    </section>

</body>
</html>
```
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Delicious Bites- Menu</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
            
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: white;
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;

        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
            
        }

        .menu-container {
            padding: 20px;
            background: #f9f9f9;
            text-align: center;
            background-image: url(bg2.jpg);
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size: cover;
        }

        .menu-container h1 {
            font-size: 2rem;
            color: #ffffff;
            margin-bottom: 15px;
        }

        .menu-items {
            display: flex;
            flex-wrap: wrap;
            gap: 15px;
            justify-content: center;
        }

        .menu-item {
            background: white;
            border: 3px solid white;
            border-radius: 20px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 295px;
            overflow: hidden;
            transition: transform 0.3s ease;
        }

        .menu-item img {
            width: 100%;
            height: 180px;
            object-fit: cover;
        }

        .menu-item:hover {
            transform: scale(1.05);
        }

        .menu-details {
            padding: 10px;
            font-family: "lucida handwriting";
        }

        .menu-details h3 {
            font-size: 1.2rem;
            color: #000000;
            margin-bottom: 8px;
        }

        .menu-details p {
            font-size: 0.9rem;
            color: #555;
            margin-bottom: 10px;
        }

        .menu-details .price {
            font-weight: bold;
            font-size: 1rem;
            color: #ff5722;
        }

        footer {
            background: #333;
            color: white;
            text-align: center;
            padding: 10px 0;
            margin-top: 10px;
        }

        footer {
            background: rgb(4, 186, 95);
            color: rgb(0, 0, 0);
            text-align: center;
            padding: px 0;
            margin-top: 180px;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.2rem;
            }

            .menu-items {
                flex-direction: column;
                gap: 20px;
            }

            .menu-item {
                width: 100%;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="1logo.webp" href="home.html" alt="The Baratie Logo">
            <div class="ltext"><h1 >Delicious Bites</h1></div>
        </div>
        
            <nav>
                <a href="home.html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>

    <div class="menu-container">
        <h1>Our Menu</h1>
        <div class="menu-items">
            <div class="menu-item">
                <img src="indian meals.webp" alt="THALI">
                <div class="menu-details">
                    <h3>Veg Meals</h3>
                    <p class="price">₹400/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1nonveg.jpeg" alt=">Non-Veg Meals">
                <div class="menu-details">
                    <h3>Non-Veg Meals</h3>
                    <p class="price">₹450/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1pulao.jpeg" alt="Veg Pulao">
                <div class="menu-details">
                    <h3>Veg Pulao</h3>
                    <p class="price">₹190/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1chicken.jpeg" alt="Chicken Briyani">
                <div class="menu-details">
                    <h3>Chicken Briyani</h3>
                    <p class="price">₹300/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="muttonbriyani.jpg" alt="Mutton Briyani">
                <div class="menu-details">
                    <h3>Mutton Briyani</h3>
                    <p class="price">₹360/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="1amburbriyani.webp" alt="Ambur Briyani">
                <div class="menu-details">
                    <h3>Ambur Briyani</h3>
                    <p class="price">₹320/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="1gheeroast.webp" alt="Chicken Ghee Roast">
                <div class="menu-details">
                    <h3>Chicken Ghee Roast</h3>
                    <p class="price">₹385/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="1gonguramutton.webp" alt=" Gongura Mutton">
                <div class="menu-details">
                    <h3>Gongura Mutton</h3>
                    <p class="price">₹255/-</p>
                </div>
            </div>

            <div class="menu-item">
                <img src="1korigassi.webp" alt="Kori Gassi">
                <div class="menu-details">
                    <h3>Kori Gassi</h3>
                    <p class="price">₹530/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1PalkattiChettinad.webp" alt=" Palkatti Chettinadu">
                <div class="menu-details">
                    <h3>Palkatti Chettinadu</h3>
                    <p class="price">₹370/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1bagarabaingan.webp" alt="Bagara Baingan">
                <div class="menu-details">
                    <h3>Bagara Baingan</h3>
                    <p class="price">₹490/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1Chemmeenmangacurry.webp" alt="Chemmeen Manga Curry">
                <div class="menu-details">
                    <h3>Chemmeen Manga Curry</h3>
                    <p class="price">₹280/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1prawncurry.jpg" alt="Prawn Curry">
                <div class="menu-details">
                    <h3>Prawn Curry</h3>
                    <p class="price">₹450/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1shikampurikebab.webp" alt="Shikampuri Kebab">
                <div class="menu-details">
                    <h3>Shikampuri Kebab</h3>
                    <p class="price">₹500/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1nanduvaruval.webp" alt="Crab Varuval">
                <div class="menu-details">
                    <h3>Crab Varuval</h3>
                    <p class="price">₹300/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1fish.webp" alt="Meen Poluchathu">
                <div class="menu-details">
                    <h3>Meen Poluchathu</h3>
                    <p class="price">₹260/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1Kaara Azhagar.webp" alt="Kaara Azhagar">
                <div class="menu-details">
                    <h3>Kaara Azhagar</h3>
                    <p class="price">₹700/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1puttu.jpg" alt="Kerala Puttu with Kadalai Curry">
                <div class="menu-details">
                    <h3>Kerala Puttu with Kadalai Curry</h3>
                    <p class="price">₹120/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1sweetidly.webp" alt="Sweet Idly">
                <div class="menu-details">
                    <h3>Sweet Idly</h3>
                    <p class="price">₹70/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1dosa.png" alt="Masala Dosa">
                <div class="menu-details">
                    <h3>Masala Dosa</h3>
                    <p class="price">₹50/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1pesarattu.webp" alt="Pesarattu">
                <div class="menu-details">
                    <h3>Pesarattu</h3>
                    <p class="price">₹60/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1paniyaram.webp" alt="Kuli Paniyaram">
                <div class="menu-details">
                    <h3>Kuli Paniyaram</h3>
                    <p class="price">₹30/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1appam.webp" alt="Appam With Coconut Milk">
                <div class="menu-details">
                    <h3>Appam With Coconut Milk</h3>
                    <p class="price">₹40/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1poori.jpeg" alt="Poori & Masala">
                <div class="menu-details">
                    <h3>Poori & Masala</h3>
                    <p class="price">₹40/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1parotta.jpeg" alt="Madurai Bun Parotta">
                <div class="menu-details">
                    <h3>Madurai Bun Parotta</h3>
                    <p class="price">₹50/-</p>
                </div>
            </div>
            <div class="menu-item">
                <img src="1vada.jpeg" alt="Medhu Vada">
                <div class="menu-details">
                    <h3>Medhu Vada</h3>
                    <p class="price">₹35/-</p>
                </div>
            </div>
        </div>
    </div>

</body>
</html>
```
```
<html>
<head>
    <title>Delicious Bites - Contact Us</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: white;
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;

        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }
        .contact-banner h1 {
            font-family: Georgia, 'Times New Roman', Times, serif;
            font-size: 2.5rem;
            color:white;
            background-image: url(bg2.jpg);
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size: cover;
        }
        .contact-section {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            padding: 30px 15px;
            background: white;
            gap: 20px;
            background-image: url(bg4.jpeg);
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size: cover;
        }
        .contact-details, .contact-form {
            flex: 1;
            max-width: 500px;
            margin: 10px;
            background: white;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 4px 4px 4px 6px rgba(0, 0, 0, 0.1);
        }
        .contact-details h2, .contact-form h2 {
            font-size: 1.8rem;
            margin-bottom: 15px;
            color: #1f1714;
            text-align: center;
        }
        .contact-details p {
            margin: 10px 0;
            font-size: 1rem;
            color: #555;
        }
        .contact-details img {
            max-width: 100%;
            border-radius: 10px;
            margin-bottom: 20px;
        }
        .contact-form input, .contact-form textarea {
            width: 100%;
            padding: 10px;
            margin: 10px 0;
            border: 1px solid #ccc;
            border-radius: 5px;
            font-size: 1rem;
        }
        .contact-form textarea {
            height: 100px;
        }
        .contact-form button {
            width: 100%;
            padding: 10px;
            background: #ff5722;
            color: white;
            font-size: 1.1rem;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            transition: background 0.3s ease;
        }
        .contact-form button:hover {
            background: #e64a19;
        }
        footer {
            background: rgb(4, 186, 95);
            color: rgb(0, 0, 0);
            text-align: center;
            padding: px 0;
            margin-top: 180px;
        }

        @media (max-width: 768px) {
            .contact-details, .contact-form {
                max-width: 100%;
            }

            .contact-banner h1 {
                font-size: 2rem;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="1logo.webp" href="home.html" alt="The Baratie Logo">
            <div class="ltext"><h1 >Delicious Bites</h1></div>
        </div>
        
            <nav>
                <a href="home.html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>

    <div class="contact-banner">
     
    

    <section class="contact-section">
        <div class="contact-details">
            <h2>Get in Touch</h2>
            <img src="1contact.jpeg" alt="Contact Us">
            <p><strong>Phone:</strong> +91 9075005279</p>
            <p><strong>Email:</strong> deliciousbites@gmail.com</p>
            <p><strong>Opens:</strong> Mon-Sun(8 AM - 10 PM)</p>
        </div>

        <div class="contact-form">
            <h2>Send Us a Message</h2>
            <form action="/submit-contact" method="POST">
                <label for="name">Full Name</label>
                <input type="text" id="name" name="name" 
                placeholder="Enter your full name" required>

                <label for="email">Email Address</label>
                <input type="email" id="email" name="email"
                 placeholder="Enter your email address" required>

                <label for="message">Message</label>
                <textarea id="message" name="message"
                 placeholder="Your message" required></textarea>

                <button type="submit">Send Message</button>
            </form>
        </div>
    </section>
   </div>
</body>
</html>
```
```
<html>
<head>
    <title>Delicious Bites- Administration</title>
    <style>
        body {
            margin: 0;
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            box-sizing: border-box;
        }

        *, *::before, *::after {
            box-sizing: inherit;
        }

        header {
            background: white;
            color: #000000;
            padding: 5px 10px;
            display: flex;
            align-items: center;
            justify-content: space-between;
            position: relative;
            height: 80px;
            overflow: hidden;
            
        }

        header nav a {
            padding-right: 10px;
            text-decoration: none;
            color: #000000;
            font-weight: bold;
            margin: 0 10px;
            transition: color 0.3s ease;
        }

        header nav a:hover {
            color: #ff5722;
        }

        .tblogo{
            display: flex;
            height: 120px;

        }

        .ltext{
            height: 95px;
            margin-top: 5%;
            font-family: Georgia, 'Times New Roman', Times, serif;
        }


        .admin-container {
            padding: 20px;
            background-image: url(bg2.jpg);
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size: cover;
            
            text-align: center;

        }

        .admin-container h1 {
            font-size: 2rem;
            color: #fffdfd;
            margin-bottom: 20px;
            
        }

        .admin-items {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }

        .admin-item {
            background: white;
            border-radius: 10px;
            border: 3px solid white;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            width: 300px;
            overflow: hidden;
            transition: transform 0.3s ease;
            text-align: left;
        }

        .admin-item img {
            width: 100%;
            height: 200px;
            object-fit: cover;
        }

        .admin-item:hover {
            transform: scale(1.05);
        }

        .admin-details {
            padding: 15px;
        }

        .admin-details h3 {
            text-align: center;
            font-size: 1.2rem;
            color: #000000;
            margin-bottom: 8px;
        }

        .admin-details p {
            font-size: 0.9rem;
            color: #555;
            margin-bottom: 10px;
        }

        footer {
            background: rgb(4, 186, 95);
            color: rgb(0, 0, 0);
            text-align: center;
            padding: px 0;
            margin-top: 180px;
        }

        @media (max-width: 768px) {
            header h1 {
                font-size: 1.2rem;
            }

            .admin-items {
                flex-direction: column;
                gap: 20px;
            }

            .admin-item {
                width: 100%;
            }

            header nav a {
                margin: 0 5px;
            }
        }
    </style>
</head>
<body>

    <header>
        <div class="tblogo">
            <img src="1logo.webp" href="home.html" alt="The Baratie Logo">
            <div class="ltext"><h1 >Delicious Bites</h1></div>
        </div>
        
            <nav>
                <a href="home.html">Home</a>
                <a href="menu.html">Menu</a>
                <a href="contact.html">Contact</a>
                <a href="admin.html">Administration</a>
           </nav>
        
    </header>
    <div class="admin-container">
        <h1>Our Administration Team</h1>
        <div class="admin-items">
            <div class="admin-item">
                <img src="1chef.png" alt="CEO">
                <div class="admin-details">
                    <h3>Chef Zane</h3>
                    <p>CEO - Leading Delicious Bites with a vision of excellence 
                    and innovation in hospitality.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="1chef1.avif" alt="Manager">
                <div class="admin-details">
                    <h3>Chef Xavier</h3>
                    <p>Manager - Ensures smooth operations and a great dining
                     experience for all guests.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="1chef2.png" alt="Master Chef">
                <div class="admin-details">
                    <h3>Chef Elisa</h3>
                    <p>Master Chef - Brings authentic Italian flavors to every dish served.</p>
                </div>
            </div>

            <div class="admin-item">
                <img src="1chef3.png" alt="Assistant Managing Director">
                <div class="admin-details">
                    <h3>Chef Edward</h3>
                    <p>Assistant Managing Director - Supporting the team with 
                    strategy and execution excellence.</p>
                </div>
            </div>
            <div class="admin-item">
                <img src="1chef4.png" alt="Assistant 1">
                <div class="admin-details">
                    <h3>Chef Chester</h3>
                    <p>Assistant 1 - Supporting the team with strategy and execution excellence.</p>
                </div>
            </div>
            <div class="admin-item">
                <img src="1chef5.png" alt="Assistant 2">
                <div class="admin-details">
                    <h3>Chef Remy</h3>
                    <p>Assistant 2 - Supporting the team with strategy and execution excellence.</p>
                </div>
            </div>
        </div>
    </div>

</body>
</html>
```

## OUTPUT:
![alt text](<Screenshot 2025-05-04 160101.png>)

![alt text](<Screenshot 2025-05-04 160135.png>)
![alt text](<Screenshot 2025-05-04 160154.png>)
![alt text](<Screenshot 2025-05-04 160213.png>)
![alt text](<Screenshot 2025-05-04 160228.png>)
![alt text](<Screenshot 2025-05-04 160251.png>)
## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
