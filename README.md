# Project Responsive Web Design using Bootstrap
## Date:12-05-2024

## AIM:
To design a responsive website for a Pharmaceutical Company using Bootstrap.


## DESIGN STEPS:

### Step 1:
Clone the repository from GitHub.

### Step 2:
Create Django Admin project.

### Step 3:
Create a New App under the Django Admin project.

### Step 4:
Insert the necessary CSS and JavaScript files as external in order to use Bootstrap.

### Step 5:
Create a HTML file and include the needed Bootstrap components.

### Step 6:
Publish the website in the LocalHost.

## PROGRAM :
home.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Home - PharmaGen Company</title>
  <!-- Bootstrap CSS -->
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
  <style>
    .navbar {
      background-color: #727cbf; 
    }
    body{
    background-image: url("bg.avif");
      background-size: cover;
      background-repeat: no-repeat;
      font-size: 20px;
    }
    footer {
      position: fixed;
      bottom: 0;
      width: 100%;
      background-color: #343a40; 
      color: rgb(238, 236, 236); 
      padding: 10px 0;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark">
    <a class="navbar-brand" href="#">PharmaGen Company</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item active">
          <a class="nav-link" href="home.html">Home <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="about.html">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="products.html">Products</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="contact.html">Contact</a>
        </li>
      </ul>
      <ul class="navbar-nav ml-auto">
        <li class="nav-item">
          <a class="nav-link" href="#">Login</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Register</a>
        </li>
      </ul>
    </div>
  </nav>

  <!-- Page Content -->
  <div class="container mt-5">
    <div class="row">
      <div class="col-md-8">
        <h1>Welcome to PharmaGen Company</h1>
        <p>your trusted source for quality healthcare products and services.</p>
        <p>we are committed to providing you with personalized care and the highest quality medications and health products. Whether you're looking for prescription medications, over-the-counter remedies, or wellness products, we're here to serve you.</p>
        <p>Explore our website to discover our range of products and services, including prescription refills, health supplements, medical equipment, and more.</p>
        <p> Thank you for choosing PharmaGen Company. Your health journey starts here.</p>
      </div>
      <div class="col-md-4">
        <img src="pharm.avif" class="img-fluid" alt="Pharmacy Image">
      </div>
    </div>
  </div>

  <!-- Footer -->
  <footer class="bg-dark text-white text-center">
    <div class="container">
      <p>&copy; 2024 PharmaGen Company. All rights reserved BY PRIYADHARSHINI.P (212223240128)</p>
    </div>
  </footer>

  <!-- Bootstrap JS -->
  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
```
about.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>About Us</title>
  <!-- Bootstrap CSS -->
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
  <style>
     .navbar {
      background-color: #727cbf; 
     }
    body {
      display: flex;
      flex-direction: column;
      min-height: 100vh;
      background-image: url("bg.avif");
      background-size: cover;
      background-repeat: no-repeat;
      font-size: 20px;
    }
    .content {
      flex: 1;
    }
    footer {
      background-color: #343a40; /* Dark background color */
      color: white; /* Text color */
      text-align: center;
      padding: 20px 0;
      width: 100%;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark">
    <a class="navbar-brand" href="#">PharmaGen Company</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item">
          <a class="nav-link" href="home.html">Home</a>
        </li>
        <li class="nav-item dropdown active">
          <a class="nav-link dropdown-toggle" href="about.html" id="navbarDropdownAbout" role="button" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">About</a>
          <div class="dropdown-menu" aria-labelledby="navbarDropdownAbout">
            <a class="dropdown-item" href="#misson">Vision</a>
            <a class="dropdown-item" href="#values">Mission</a>
            <a class="dropdown-item" href="#services">Values</a>
            <!-- Add more subheadings as needed -->
          </div>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="products.html">Products</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="contact.html">Contact</a>
        </li>
      </ul>
    </div>
  </nav>

  <!-- Page Content -->
  <div class="container mt-5 content">
    <div class="row">
      <div class="col-md-12">
        <h1>About Us</h1>
        <div id="mission">
          <h2>Our Mission</h2>
          <p>Our mission is to provide accessible, compassionate, and personalized healthcare services.We strive to empower healthier lives by offering quality medication. </p>
        </div>
        <div id="values">
          <h2>Our Values</h2>
          <ul>
            <li>Customer-Centric: We prioritize our customers' needs and strive to exceed their expectations.</li>
            <li>Integrity: We uphold the highest standards of honesty, ethics, and professionalism.</li>
            <li>Quality: We are committed to delivering products and services of the highest quality.</li>
            <li>Community Engagement: We actively support and contribute to the well-being of the communities we serve.</li>
          </ul>
        </div>
        <div id="mission">
            <h2>Our Team</h2>
            <p>Our team consists of experienced pharmacists, pharmacy technicians, and healthcare professionals who are dedicated to providing exceptional care and service.</p>
          </div>
        <!-- Add more subheadings as needed -->
      </div>
    </div>
  </div>

  <!-- Footer -->
  <footer>
    <div class="container">
      <p>&copy; 2024 PharmaGen Company. All rights reserved BY PRIYADHARSHINI.P (212223240010)</p>
    </div>
  </footer>

  <!-- Bootstrap JS -->
  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
```
products.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Products - PharmaGen Company</title>
  <!-- Bootstrap CSS -->
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
  <style>
    .navbar {
      background-color: #727cbf; 
    }
    body {
      display: flex;
      flex-direction: column;
      min-height: 100vh;
      margin: 0;
      padding: 0;
      background: url("bg.avif") no-repeat center center fixed;
      background-size: cover;
    }
    .content {
      flex: 1;
    }
    footer {
      background-color: rgba(0, 0, 0, 0.8); /* Dark background color with opacity */
      color: white; /* Text color */
      text-align: center;
      padding: 20px 0;
      width: 100%;
    }
  </style>
</head>
<body>

  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark">
    <a class="navbar-brand" href="#">PharmaGen Company</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item">
          <a class="nav-link" href="home.html">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="about.html">About</a>
        </li>
        <li class="nav-item active">
          <a class="nav-link" href="products.html">Products <span class="sr-only">(current)</span></a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="contact.html">Contact</a>
        </li>
      </ul>
      <ul class="navbar-nav ml-auto">
        <li class="nav-item">
          <a class="nav-link" href="#">Login</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="#">Register</a>
        </li>
      </ul>
    </div>
  </nav>

  <!-- Page Content -->
  <div class="container mt-5 content">
    <div class="row">
      <div class="col-md-12">
        <h1>Our Products</h1>
        <div class="card-deck">
          <div class="card">
            <img src="image1.png" class="card-img-top" alt="Product 1" width="200" height="200">
            <div class="card-body">
              <h5 class="card-title">Himalaya Diabecon </h5>
              <p class="card-text">Himalaya Diabecon tablets are an Ayurvedic proprietary medicine that is carefully designed with a blend of herbs known for their anti-diabetic properties. </p>
              <a href="#" class="btn btn-primary">Buy Now</a>
            </div>
          </div>
          <div class="card">
            <img src="image2.png" class="card-img-top" alt="Product 2" width="200" height="200">
            <div class="card-body">
              <h5 class="card-title">Iodex Ultra Gel</h5>
              <p class="card-text">odex Ultra Gel is a new and improved formula for faster pain relief. The gel penetrates deeper into the muscles and helps relax the body pain</p>
              <a href="#" class="btn btn-primary">Buy Now</a>
            </div>
          </div>
          <div class="card">
            <img src="image3.png" class="card-img-top" alt="Product 3" width="200" height="200">
            <div class="card-body">
              <h5 class="card-title">Apollo Life Aloe Vera Juice</h5>
              <p class="card-text">The Apollo Life Aloe Vera Juice is a premium quality beverage extracted from the succulent inner gel of Aloe vera leaves, ensuring maximum potency and purity.</p>
              <a href="#" class="btn btn-primary">Buy Now</a>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Footer -->
  <footer>
    <div class="container">
      <p>&copy; 2024 PharmaGen Company. All rights reserved BY PRIYADHARSHINI.P (212223240128)</p>
    </div>
  </footer>

  <!-- Bootstrap JS -->
  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
```
contact.html
```
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Contact Us - PharmaGen Company</title>
  <!-- Bootstrap CSS -->
  <link href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css" rel="stylesheet">
</head>
<body>
<style>      
.navbar {
        background-color: #727cbf; 
}
body{
    background-image: url("bg.avif");
      background-size: cover;
      background-repeat: no-repeat;
      font-size: 15px;
}
</style>
  <!-- Navbar -->
  <nav class="navbar navbar-expand-lg navbar-dark">
    <a class="navbar-brand" href="#">PharmaGen Company</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
      <span class="navbar-toggler-icon"></span>
    </button>

    <div class="collapse navbar-collapse" id="navbarSupportedContent">
      <ul class="navbar-nav mr-auto">
        <li class="nav-item">
          <a class="nav-link" href="home.html">Home</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="about.html">About</a>
        </li>
        <li class="nav-item">
          <a class="nav-link" href="products.html">Products</a>
        </li>
        <li class="nav-item active">
          <a class="nav-link" href="contact.html">Contact <span class="sr-only">(current)</span></a>
        </li>
      </ul>
    </div>
  </nav>

  <!-- Page Content -->
  <div class="container mt-5">
    <div class="row">
      <div class="col-md-8">
        <h1>Contact Us</h1>
        <p>For any inquiries or feedback, please fill out the form below and we will get back to you as soon as possible.</p>
        <form>
          <div class="form-group">
            <label for="name">Your Name</label>
            <input type="text" class="form-control" id="name" placeholder="Enter your name">
          </div>
          <div class="form-group">
            <label for="email">Your Email</label>
            <input type="email" class="form-control" id="email" placeholder="Enter your email">
          </div>
          <div class="form-group">
            <label for="message">Message</label>
            <textarea class="form-control" id="message" rows="5" placeholder="Enter your message"></textarea>
          </div>
          <button type="submit" class="btn btn-primary">Submit</button>
        </form>
      </div>
      <div class="col-md-4">
        <h2>PharmaGen Company</h2>
        <address>
          <strong>Address:</strong><br>
          156 sathyanagar 2nd st,velachery, Chennai<br>
          India, 600042<br><br>
          <strong>Email:</strong><br>
          <p>For queries related to Online orders.Please contact us at: contactusnow@pharmagen.org</p>
          <p>For queries related to Apollo Pharmacy Store experience.Please contact us at: customerservice@pharmagen.org</p><br><br>
          <strong>Phone:</strong><br>
          <p>Main Office: 8148090261</p>
          <p>Customer Service: 044-76437863</p>
        </address>
      </div>
    </div>
  </div>
  <body background="a.png" style="background-repeat: no-repeat; background-size: cover;">


  <!-- Footer -->
  <footer class="bg-dark text-white text-center py-4 mt-5">
    <p>&copy; 2024 PharmaGen Company. All rights reserved  BY PRIYADHARSHINI.P (212223240128)</p>
  </footer>

  <!-- Bootstrap JS -->
  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/popper.js@1.16.1/dist/umd/popper.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>
</html>
```

## OUTPUT:
![image](https://github.com/priyadharshini210/Pharma/assets/148514638/6e58f598-4549-4d39-b0c7-d4ec0c0a8492)
![image](https://github.com/priyadharshini210/Pharma/assets/148514638/a444188e-2a1e-4d19-8301-c60d3b190779)
![Screenshot (105)](https://github.com/priyadharshini210/Pharma/assets/148514638/d2d0ec55-d1a5-4d3c-b182-c8823ed5be51)
![image](https://github.com/priyadharshini210/Pharma/assets/148514638/fde5b3f3-7878-4937-839f-2a7baf847376)


## CODE:
![image](https://github.com/priyadharshini210/Pharma/assets/148514638/b950e13d-6d52-4d31-afac-86a3c7cc6b7e)


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
