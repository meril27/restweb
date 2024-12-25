# Ex.07 Restaurant Website
## Date:

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
home.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Golden Spoon Café</title>
    <style>
        body {
          font-family: Arial, sans-serif;
          margin: 0;
          padding: 0;
          background-color: #c4ba2b;
    
        }
        header {
          background-color:#80c2a3;
          padding: 20px;
          text-align: center;
          border-bottom: 2px solid #6db5bd;
        }
        header img {
          height: 100px;
          width: 200px;
          vertical-align: middle;
        }
        header h1 {
          display: inline;
          margin-left: 10px;
          font-size: 24px;
          color: #6a103c;
        }
        nav {
          background-color: #333;
          overflow: hidden;
        }
        nav a {
          color: white;
          padding: 14px 20px;
          text-decoration: none;   
          display: block;
          float:left;
          
        }
        nav a:hover {
          background-color: #575757;
    
        }
        .content {
          display: flex;
          justify-content: space-around;
          padding: 20px;
        }
        .content div {
          background-color: #f8f8f8;
          padding: 20px;
          margin: 10px;
          flex: 1;
          text-align: center;
          border-radius: 8px;
          box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
    
        }
        footer {
          text-align: center;
          padding: 5px;
          background-color: #0f0e0c;
          color: rgb(187, 188, 79);
          position: absolute;
          bottom: 0;
          width: 100%;
        }
      </style>
</head>
<body>
    <section class="intro">
    <h1 align="center">Welcome to Our Café </h1>
    <p align="center">Enjoy a variety of delicious dishes, prepared with fresh ingredients!</p>
</section>
<header>
    <img src="c:\Users\admin\restweb\website\restapp\static\logo.jpeg" alt="Golden Spoon Café" height="100" width="100">
    <br><br>
    <h1><font face="goudy old style italic"size="7">Golden Spoon Café</font></h1>
  </header>
  <nav>
    <a href="home.html" >Home</a>
    <a href="menu.html">Menu</a>
    <a href="administration.html">Administration</a>
    <a href="contact.html">Contact Us</a>
  </nav>
  <div class="content">
    <div>
      <h3>Our New Menu</h3>
      <img src="c:\Users\admin\restweb\website\restapp\static\menu.webp" alt="Menu img 1" height="200" width="300">
      <p>Discover our latest dishes with unique flavors.</p>
      <a href="menu.html">See our menu</a>
    </div>
    <div>
      <h3>Book a Table</h3>
      <img src="c:\Users\admin\restweb\website\restapp\static\booktable.jpg" alt="Menu img 1" height="200" width="300">
      <p>Reserve your spot to enjoy a delightful dining experience.</p>
      <a href="contact.html">Book now</a>
    </div>
    <div>
      <h3>Opening Hours</h3>
      <img src="c:\Users\admin\restweb\website\restapp\static\openhours.jpg" alt="Menu img 1" height="200" width="300">
      <p>Mon-Fri: 6am - 10pm<br><br>Sat: 2pm - 11pm<br><br>Sun: 2pm - 9pm</p>
    </div>
  </div>
  <footer>
    <p>Designed by MERIL GOLDLINA A (24007299)</p>
  </footer>
</body>
</html>
</html>
```
```
menu.html

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="styles.css">
    <title>Golden Spoon Café</title>
    <style>
        body {
          font-family: Arial, sans-serif;
          margin: 0;
          padding: 0;
          background-color: #c4ba2b;
        }

        header {
          background-color: #80c2a3;
          padding: 20px;
          text-align: center;
          border-bottom: 2px solid #6db5bd;
        }

        header img {
          height: 100px;
          width: 200px;
          vertical-align: middle;
        }

        header h1 {
          display: inline;
          margin-left: 10px;
          font-size: 24px;
          color: #6a103c;
          font-family: "Goudy Old Style", sans-serif;
        }

        header h2 {
          font-size: 18px;
          font-family: "Goudy Old Style", sans-serif;
          color: #333;
        }

        nav {
          background-color: #333;
          overflow: hidden;
        }

        nav a {
          color: white;
          padding: 14px 20px;
          text-decoration: none;
          display: block;
          float: left;
        }

        nav a:hover {
          background-color: #575757;
        }

        section {
          padding: 20px;
        }

        h2 {
          text-align: center;
          margin-bottom: 20px;
        }

        /* Flexbox layout for the menu items */
        .menu-items {
          display: flex;
          flex-wrap: wrap;
          justify-content: space-between;
          padding: 20px;
        }

        .menu-item {
          background-color: #f8f8f8;
          padding: 20px;
          margin: 10px;
          width: 23%;
          text-align: center;
          border-radius: 8px;
          box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
          box-sizing: border-box;
        }

        .menu-item img {
          width: 100%;
          height: auto;
          border-radius: 8px;
        }

        /* Responsive Design for smaller screens */
        @media (max-width: 768px) {
          .menu-item {
            width: 48%;
          }
        }

        @media (max-width: 480px) {
          .menu-item {
            width: 100%;
          }
        }

        footer {
          text-align: center;
          padding: 5px;
          background-color: #0f0e0c;
          color: rgb(187, 188, 79);
          position: relative;
          bottom: 0;
          width: 100%;
        }
    </style>
</head>
<body>
<header>
    <img src="c:\Users\admin\restweb\website\restapp\static\logo.jpeg" alt="Golden Spoon Café Logo" height="100" width="100">
    <br><br>
    <h1><font face="goudy old style italic"size="8">Golden Spoon Café</font></h1>
    <h2><font size="6">Menu</font></h2>
</header>

<nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="administration.html">Administration</a>
    <a href="contact.html">Contact Us</a>
</nav>

<section id="menu">
    <h2>Our Delicious Menu</h2>
    <div class="menu-items">
        <!-- Item 1 -->
        <div class="menu-item">
          <img src="c:\Users\admin\restweb\website\restapp\static\chicken pizza.jpg" alt="Chicken Pizza">
            <h3>Chicken Pizza</h3>
            <p>Price: $120.00</p>
        </div>
        <!-- Item 2 -->
        <div class="menu-item">
            <img src="c:\Users\admin\restweb\website\restapp\static\pizza-margherita-wooden-background-top-view-flyer-poster-restaurants-pizzerias_120962-7.jpg" alt="Margherita Pizza">
            <h3>Margherita Pizza</h3>
            <p>Price: $140.00</p>
        </div>
        <!-- Item 3 -->
        <div class="menu-item">
            <img src="c:\Users\admin\restweb\website\restapp\static\VeggieBurger_RECIPE_IG_021320_516_VOG_final.webp" alt="Veggie Burger">
            <h3>Veggie Burger</h3>
            <p>Price: $80.00</p>
        </div>
        <!-- Item 4 -->
        <div class="menu-item">
            <img src="c:\Users\admin\restweb\website\restapp\static\Noodles-with-chilli-oil-eggs-6ec34e9.jpg" alt="Fried Noodles">
            <h3>Fried Noodles</h3>
            <p>Price: $100.00</p>
        </div>
        <!-- Item 5 -->
        <div class="menu-item">
            <img src="c:\Users\admin\restweb\website\restapp\static\chicken lollipop.jpg" alt="Chicken Lollipop">
            <h3>Chicken Lollipop</h3>
            <p>Price: $90.00</p>
        </div>
        <!-- Item 6 -->
        <div class="menu-item">
            <img src="c:\Users\admin\restweb\website\restapp\static\Popcorn-Crusted-Fish-Fingers.jpg" alt="Fish Fingers">
            <h3>Fish Fingers</h3>
            <p>Price: $130.00</p>
        </div>
        <!-- Item 7 -->
        <div class="menu-item">
            <img src="c:\Users\admin\restweb\website\restapp\static\paneerL.jpg" alt="Paneer Butter Masala">
            <h3>Paneer Butter Masala</h3>
            <p>Price: $85.00</p>
        </div>
        <!-- Item 8 -->
        <div class="menu-item">
            <img src="c:\Users\admin\restweb\website\restapp\static\white sauce pasta.jpg" alt="White Sauce Pasta">
            <h3>White Sauce Pasta</h3>
            <p>Price: $160.00</p>
        </div>
        <!-- Item 9 -->
        <div class="menu-item">
            <img src="c:\Users\admin\restweb\website\restapp\static\decadent-chocolate-milkshake-satisfying-32-ratio_1000124-6734.jpg" alt="Butter-chocolate Milkshake">
            <h3>Butter-chocolate Milkshake</h3>
            <p>Price: $110.00</p>
        </div>
        <!-- Item 10 -->
        <div class="menu-item">
            <img src="c:\Users\admin\restweb\website\restapp\static\veg-fried-rice-recipe-500x500.webp" alt=" VEG Fried Rice">
            <h3>VEG Fried Rice</h3>
            <p>Price: $110.00</p>
        </div>
        <!-- Item 11 -->
        <div class="menu-item">
            <img src="c:\Users\admin\restweb\website\restapp\static\sushi.jpg" alt="Sushi">
            <h3>Sushi</h3>
            <p>Price: $190.00</p>
        </div>
        <!-- Item 12 -->
        <div class="menu-item">
            <img src="c:\Users\admin\restweb\website\restapp\static\mutton-biriyani.jpeg" alt="Mutton Briyani">
            <h3>Mutton Briyani</h3>
            <p>Price: $200.00</p>
        </div>
    </div>
</section>

<footer>
    <p>Designed by MERIL GOLDLINA A (24007299)</p>
</footer>
</body>
</html>
```
```
administration.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Administration - Golden Spoon Café</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #c4ba2b;
    }

    header {
      background-color: #80c2a3;
      padding: 20px;
      text-align: center;
      border-bottom: 2px solid #6db5bd;
    }

    header img {
      height: 100px;
      width: 200px;
      vertical-align: middle;
    }

    header h1 {
      display: inline;
      margin-left: 10px;
      font-size: 48px;
      color: #69133c;
      font-family: 'Goudy Old Style', serif;
      font-style: italic;
    }

    header h2 {
      font-size: 24px;
      font-family: 'Goudy Old Style', serif;
      color: #333;
    }

    nav {
      background-color: #333;
      overflow: hidden;
    }

    nav a {
      color: white;
      padding: 14px 20px;
      text-decoration: none;
      display: block;
      float: left;
      transition: background-color 0.3s ease;
    }

    nav a:hover {
      background-color: #575757;
    }

    section {
      padding: 20px;
    }

    h2 {
      text-align: center;
      margin-bottom: 20px;
    }

    .administration {
      display: flex;
      flex-wrap: wrap;
      justify-content: space-between;
      padding: 20px;
    }

    .chef {
      background-color: #f8f8f8;
      padding: 20px;
      margin: 10px;
      width: 23%; /* Adjust width to make sure they fit side by side */
      text-align: center;
      border-radius: 8px;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      box-sizing: border-box;
      transition: transform 0.3s ease; /* Optional: for hover effect */
    }

    .chef img {
      max-width: 100%;
      height: auto;
      border-radius: 8px;
    }

    @media (max-width: 768px) {
      .chef {
        width: 48%; /* On smaller screens, reduce to 2 per row */
      }
    }

    @media (max-width: 480px) {
      .chef {
        width: 100%; /* On mobile screens, display one per row */
      }
    }

    .chef:hover {
      transform: scale(1.05); /* Optional: zoom effect on hover */
    }

    footer {
  text-align: center;
  padding: 30px;  /* Increased padding for more height */
  background-color: #0f0e0c;
  color: rgb(187, 188, 79);
  position: relative;
  bottom: 0;
  width: 100%;
}

  </style>
</head>
<body>
  <header>
    <img src="c:\Users\admin\restweb\website\restapp\static\logo.jpeg" alt="Golden Spoon Café Logo" height="100" width="100"><br><br>
    <h1>Golden Spoon Café</h1><br>
    <h2><font size="6">Administration</font></h2>
  </header>
  <nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="administration.html">Administration</a>
    <a href="contact.html">Contact Us</a>
  </nav>
  <section id="administration">
    <h2>ABOUT US</h2>
    <div class="administration">
      <div class="chef">
        <img src="c:\Users\admin\restweb\website\restapp\static\360_F_899322095_66CYDyDXIc8y0OCg7kpB0FvicVzVGcuE.jpg" alt="Dr. Chef Meril">
        <h3>Dr. Chef Meril</h3>
        <p>FOUNDER</p>
      </div>
      <div class="chef">
        <img src="c:\Users\admin\restweb\website\restapp\static\360_F_632778789_Kjqi8QZ3dYyp9lEWwgP4NrZCp9anb4dl.jpg" alt="Chef Keerthika">
        <h3>Chef Keerthika</h3>
        <p>CO-FOUNDER</p>
      </div>
      <div class="chef">
        <img src="c:\Users\admin\restweb\website\restapp\static\beautiful-korean-chef-girl-is-ready-cook-food-restaurant-kitchen_148840-14836.jpg" alt="Chef Briney">
        <h3>Chef Briney</h3>
        <p>MANAGER</p>
      </div>
      <div class="chef">
        <img src="c:\Users\admin\restweb\website\restapp\static\unnamed.jpg" alt="Dr. Chef Damu">
        <h3>Dr. Chef Damu</h3>
        <p>ASSISTANT MANAGER</p>
      </div>
      <!-- Centered Chef Cards -->
      <div class="chef">
        <img src="c:\Users\admin\restweb\website\restapp\static\channels4_profile.jpg" alt="Chef Venkatesh Bhat">
        <h3>Chef Venkatesh Bhat</h3>
        <p>SENIOR MASTER CHEF</p>
      </div>

      <div class="chef">
        <img src="c:\Users\admin\restweb\website\restapp\static\download.jpeg" alt="Chef Sivaangi Krishnakumar">
        <h3>Chef Sivaangi Krishnakumar</h3>
        <p>JUNIOR CHEF</p>
      </div>
</div>
</section>
<footer>
Designed by MERIL GOLDLINA A (24007299)
</footer>
</body>
</html>
```
```
contact.html

<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact - Golden Spoon Café</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #c4ba2b;
    }

    header {
      background-color: #80c2a3;
      padding: 20px;
      text-align: center;
      border-bottom: 2px solid #6db5bd;
    }

    header img {
      height: 100px;
      width: 200px;
      vertical-align: middle;
    }

    header h1 {
      display: inline;
      margin-left: 10px;
      font-size: 48px;
      color: #69133c;
      font-family: 'Goudy Old Style', serif;
      font-style: italic;
    }

    header h2 {
      font-size: 24px;
      font-family: 'Goudy Old Style', serif;
      color: #333;
    }

    nav {
      background-color: #333;
      overflow: hidden;
    }

    nav a {
      color: white;
      padding: 14px 20px;
      text-decoration: none;
      display: block;
      float: left;
      transition: background-color 0.3s ease;
    }

    nav a:hover {
      background-color: #575757;
    }

    section {
      padding: 20px;
    }

    h2 {
      text-align: center;
      margin-bottom: 20px;
    }

    footer {
      text-align: center;
      padding: 10px;
      background-color: #0f0e0c;
      color: rgb(187, 188, 79);
      position: relative;
      bottom: 0;
      width: 100%;
    }

    .contact {
      text-align: center;
      color: rgb(55, 203, 45);
      margin-top: 30px;
    }

    .contact h1 {
      color: rgb(230, 92, 129);
    }

    .contact h4 {
      color: rgb(30, 149, 157);
    }

    .contact p {
      color: rgb(18, 148, 41);
    }
  </style>
</head>
<body>
  <header>
    <img src="static/logo.jpeg" alt="Golden Spoon Café Logo" height="100" width="100"><br><br>
    <h1>Golden Spoon Café</h1>
    <h2><font size="5">Contact Us</font></h2>
  </header>

  <nav>
    <a href="home.html">Home</a>
    <a href="menu.html">Menu</a>
    <a href="administration.html">Administration</a>
    <a href="contact.html">Contact Us</a>
  </nav>

  <section id="contact" class="contact">
    <h1>Contact:</h1>
    <h4>+91 6098345679<br> Email: goldenspoon@gmail.com</h4>
    <p>
      Address: B-(3/80) Gandhi Nagar, Junction road, Nagercoil<br>
      Nagercoil 629001<br><br><br>
      Contact us to place your order<br><br>
    </p>
    <hr>
    <p>Savor the flavor, embrace the experience!</p>
  </section><br>

  <footer>
    <p>&copy; 2024 GOLDENSPPON. All rights reserved. | <a href="home.html">Back to Home</a></p>
    Designed by MERIL GOLDLINA A (24007299)
  </footer>
</body>
</html>
```
## OUTPUT:
![alt text](<Screenshot 2024-12-26 001108.png>)
![alt text](<Screenshot 2024-12-26 001638.png>)
![alt text](<Screenshot 2024-12-26 001716.png>)
![alt text](<Screenshot 2024-12-26 001946.png>)
![alt text](<Screenshot 2024-12-26 002016.png>)
![alt text](<Screenshot 2024-12-26 002140.png>)

## RESULT:
The program for designing software company website using HTML and CSS is completed successfully.
