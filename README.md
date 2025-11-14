# Project Responsive Web Design using Bootstrap
## Date: 14-11-2025

## AIM:
To create a simplified clone of Dribbble (https://dribbble.com/) landing page.


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
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>A Dribbble</title>
    
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">

    <style>
        .navbar { background-color: black; }
        .navbar-brand { font-weight: 700; color: white !important; }
        .nav-link { color: rgba(255, 255, 255, 0.85) !important; }
        .nav-link:hover { color: white !important; }
        .hero-section { background-color: #f5f5f5; padding: 100px 0; text-align: center; }

        .shot-card {
            border-radius: 8px; overflow: hidden; margin-bottom: 20px;
            transition: transform 0.3s ease; border: none;
        }
        .shot-card:hover { transform: translateY(-5px); }

        .shot-image { height: 200px; object-fit: cover; width: 100%; }
        .user-avatar { width: 40px; height: 40px; border-radius: 50%; object-fit: cover; }

        .section-title {
            font-weight: 700; margin-bottom: 40px; position: relative; display: inline-block;
        }
        .section-title:after {
            content: ''; position: absolute; width: 50%; height: 3px; background-color: black;
            bottom: -10px; left: 25%;
        }

        footer { background-color: #333; color: white; padding: 30px 0; margin-top: 50px; }
    </style>
</head>

<body>

    <!-- NAVBAR -->
    <nav class="navbar navbar-expand-lg navbar-dark sticky-top">
        <div class="container">
            <a class="navbar-brand" href="#"><i class="fas fa-basketball-ball me-2"></i>Dribbble</a>
            <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarNav">
                <ul class="navbar-nav ms-auto">
                    <li class="nav-item"><a class="nav-link" href="#">Inspiration</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Find Work</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Learn Design</a></li>
                    <li class="nav-item"><a class="nav-link" href="#">Go Pro</a></li>
                    <li class="nav-item ms-lg-3 mt-2 mt-lg-0">
                        <button class="btn btn-outline-light btn-sm">Sign in</button>
                    </li>
                    <li class="nav-item ms-lg-2 mt-2 mt-lg-0">
                        <button class="btn btn-light btn-sm">Sign up</button>
                    </li>
                </ul>
            </div>
        </div>
    </nav>

    <!-- HERO -->
    <section class="hero-section">
        <div class="container">
            <h1 class="display-4 fw-bold mb-4">Discover the world's top designers & creatives</h1>
            <p class="lead mb-5">Shots is the leading destination to find & showcase creative work and home to the world's best design professionals.</p>
            <button class="btn btn-primary btn-lg px-4 me-2">Sign up</button>
            <a href="#" class="btn btn-outline-primary btn-lg px-4">Learn more</a>
        </div>
    </section>

    <!-- POPULAR SHOTS WITH YOUR IMAGES -->
    <section class="py-5">
        <div class="container">
            <h2 class="text-center section-title">Popular Shots</h2>
            <div class="row">

                <div class="col-md-6 col-lg-3">
                    <div class="card shot-card shadow-sm">
                        <img src="design1.jpeg" class="shot-image" alt="Design Poster Graphic">
                        <div class="card-body"><h6 class="mb-0">Rafiz Studio</h6></div>
                    </div>
                </div>

                <div class="col-md-6 col-lg-3">
                    <div class="card shot-card shadow-sm">
                        <img src="design2.jpeg" class="shot-image" alt="Graphic Template">
                        <div class="card-body"><h6 class="mb-0">ThreeDee</h6></div>
                    </div>
                </div>

                <div class="col-md-6 col-lg-3">
                    <div class="card shot-card shadow-sm">
                        <img src="design3.jpeg" class="shot-image" alt="UI UX Design">
                        <div class="card-body"><h6 class="mb-0">Nixito</h6></div>
                    </div>
                </div>

                <div class="col-md-6 col-lg-3">
                    <div class="card shot-card shadow-sm">
                        <img src="design4.jpeg" class="shot-image" alt="Portfolio Layout">
                        <div class="card-body"><h6 class="mb-0">Ziko</h6></div>
                    </div>
                </div>

                <div class="col-md-6 col-lg-3">
                    <div class="card shot-card shadow-sm">
                        <img src="design5.png" class="shot-image" alt="Logo Collection">
                        <div class="card-body"><h6 class="mb-0">Showit</h6></div>
                    </div>
                </div>

            </div>
        </div>
    </section>

    <!-- CTA -->
    <section class="py-5 text-center">
        <div class="container">
            <h2 class="mb-4">Ready to showcase your creative work?</h2>
            <p class="lead mb-4">Join the world's leading community for creatives</p>
            <button class="btn btn-primary btn-lg px-5">Get Started</button>
        </div>
    </section>

    <!-- FOOTER -->
    <footer>
        <div class="container">
            <div class="row">
                <div class="col-md-6"><p class="mb-0">&copy; All rights reserved</p></div>
                <div class="col-md-6 text-md-end">
                    <p class="mb-0">Created by <strong>Jagannivash</strong></p>
                </div>
            </div>
        </div>
    </footer>

<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>

```

## OUTPUT:
<img width="1919" height="992" alt="Screenshot 2025-11-14 183328" src="https://github.com/user-attachments/assets/be3cd45e-03ee-4fb9-a1bb-aa4b3779e6fe" />


## RESULT:
The Project for responsive web design using Bootstrap is completed successfully.
