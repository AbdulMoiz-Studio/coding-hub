# coding-hub
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Coding Hub</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        /* Global Styles */
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background-color: #121212;
            color: #ffffff;
            line-height: 1.6;
        }

        header {
            background-color:transparent ;
            padding: 1rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo h1 {
            font-family: 'Roboto', sans-serif;
            font-size: 1.8rem;
            margin: 0;
            color: #00bcd4;
        }

        nav ul {
            list-style: none;
            padding: 0;
            margin: 0;
            display: flex;
        }

        nav ul li {
            margin-left: 1.5rem;
        }

        nav ul li a {
            color: #ffffff;
            text-decoration: none;
            font-weight: bold;
        }

        nav ul li a:hover {
            color: #00bcd4;
        }

        .contact-button {
            background-color: #00bcd4;
            color: #121212;
            border: none;
            padding: 0.8rem 1.5rem;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
            text-decoration: none;
            border-radius: 10px;
        }

        .contact-button:hover {
            background-color: #008c9e;
        }

        .hero {
             
            background-blend-mode:soft-light;
            height: 55vh;
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            text-align: center;
        }


        .hero h2 {
            font-family: 'Roboto', sans-serif;
            font-size: 2.5rem;
        }

        .hero p {
            font-size: 1.2rem;
        }

        .cta-button {
            margin-top: 1rem;
            background-color: #00bcd4;
            color: #121212;
            border: none;
            border-radius: 10px;
            padding: 0.8rem 1.5rem;
            font-size: 1rem;
            font-weight: bold;
            cursor: pointer;
        }

        .cta-button:hover {
            background-color: #008c9e;
        }

        .about {
            display: flex;
            justify-content: space-around;
            align-items: center;
            flex-wrap: wrap;
            background-color: #1e1e1e;
            padding: 2rem;
            border-radius: 10px;
        }

        .about img {
            width: 400px;
            height: 400px;
            max-width: 600px;
            border-radius: 10px;
            margin-bottom: 1rem;
        }

        .about-text {
            max-width: 600px;
        }

        .about-text h2 {
            text-align: left;
        }

        section {
            padding: 4rem 2rem;
        }

        h2 {
            font-family: 'Roboto', sans-serif;
            color: #00bcd4;
            font-size: 2rem;
            margin-bottom: 1rem;
            text-align: center;
        }

        p {
            font-family: Arial, sans-serif;
            color: #d0d0d0;
            text-align: center;
            margin-bottom: 2rem;
        }

        .language-cards {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            flex-wrap: wrap;
        }

        .card {
            background-color: #1e1e1e;
            padding: 1.5rem;
            border: 1px solid #00bcd4;
            border-radius: 5px;
            text-align: center;
            width: 250px;
        }

        .card h3 {
            font-family: 'Roboto', sans-serif;
            color: #00bcd4;
        }

        .card p {
            color: #d0d0d0;
        }

        .features {
    background-color: #1e1e1e;
    padding: 4rem 2rem;
    text-align: center;
}

.features h2 {
    color: #00bcd4;
    font-family: 'Roboto', sans-serif;
    margin-bottom: 2rem;
}

.features-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 2rem;
}

.feature-card {
    background-color: #2a2a2a;
    padding: 2rem;
    border: 1px solid #00bcd4;
    border-radius: 10px;
    width: 300px;
    text-align: center;
}

.feature-card h3 {
    color: #00bcd4;
    font-family: 'Roboto', sans-serif;
    margin-bottom: 1rem;
}

.feature-card p {
    color: #d0d0d0;
    font-family: Arial, sans-serif;
}

.success-stories {
    background-color: #121212;
    padding: 4rem 2rem;
    text-align: center;
}

.success-stories h2 {
    color: #00bcd4;
    font-family: 'Roboto', sans-serif;
    margin-bottom: 2rem;
}

.stories-container {
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
    gap: 2rem;
}

.story-card {
    background-color: #2a2a2a;
    padding: 2rem;
    border: 1px solid #00bcd4;
    border-radius: 10px;
    width: 300px;
    text-align: center;
}

.story-card h3 {
    color: #00bcd4;
    font-family: 'Roboto', sans-serif;
    margin-bottom: 1rem;
}

.story-card p {
    color: #d0d0d0;
    font-family: Arial, sans-serif;
}


        
        footer {
            background-color: #1e1e1e;
            text-align: center;
            padding: 1rem;
            margin-top: 2rem;
        }

        footer p {
            color: #808080;
            margin: 0;
        }

        .social-links a {
            color: #00bcd4;
            margin: 0 0.5rem;
            text-decoration: none;
        }

        .social-links a:hover {
            color: #008c9e;
        }

        form label, form input, form textarea, form button {
            display: block;
            width: 100%;
            margin-bottom: 1rem;
        }

        form input, form textarea {
            padding: 0.5rem;
            background-color: #1e1e1e;
            color: #ffffff;
            border: 1px solid #00bcd4;
            border-radius: 5px;
        }

        form button {
            background-color: #00bcd4;
            color: #121212;
            border: none;
            padding: 0.8rem 1.5rem;
            font-weight: bold;
            cursor: pointer;
        }

        form button:hover {
            background-color: #008c9e;
        }
    </style>
</head>
<body>
    <!-- Header Section -->
    <header>
        <div class="logo">
            <h1>Coding Hub</h1>
        </div>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#about">About Us</a></li>
                <li><a href="#learn">Learn</a></li>
                <li><a href="#profile">Profile</a></li>
            </ul>
        </nav>
        <a href="#Contact" class="contact-button">Get In Touch</a>
    </header>

    <!-- Hero Section -->
    <section id="home" class="hero">
        <h2>Welcome to Coding Hub</h2>
        <p>Master Coding with Ease at Coding Hub</p>
        <a href="#learn" class="cta-button">Get Started</a>
    </section>

    <!-- About Us Section -->
    <section id="about" class="about">
        <div class="about-image">
            <img src="about.jpg" alt="About Coding Hub">
        </div>
        <div class="about-text">
            <h2>About Us</h2>
            <p>At Coding Hub, we believe coding is the key to the future. Our mission is to provide aspiring developers and enthusiasts with the resources they need to succeed in the tech world.</p>
            <p>From hands-on coding exercises to real-world projects, Coding Hub is the ultimate platform to enhance your programming skills.</p>
        </div>
    </section>


    <!-- Learn Section -->
    <section id="learn" class="learn">
        <h2>Learn</h2>
        <div class="language-cards">
            <div class="card">
                <h3>Python</h3>
                <p>Start with the basics of Python programming.</p>
            </div>
            <div class="card">
                <h3>JavaScript</h3>
                <p>Learn how to make dynamic and interactive web pages.</p>
            </div>
            <div class="card">
                <h3>HTML & CSS</h3>
                <p>Master the building blocks of web development.</p>
            </div>
            <div class="card">
                <h3>Java</h3>
                <p>Dive into object-oriented programming with Java.</p>
            </div>
        </div>
    </section>

      <!-- Features Section -->
    <section id="features" class="features">
        <h2>Why Choose Us?</h2>
        <div class="features-container">
            <div class="feature-card">
                <h3>Interactive Lessons</h3>
                <p>Learn coding through interactive, engaging tutorials designed for all skill levels.</p>
            </div>
            <div class="feature-card">
                <h3>Real-World Projects</h3>
                <p>Build real-world projects to gain hands-on experience and boost your portfolio.</p>
            </div>
            <div class="feature-card">
                <h3>Expert Support</h3>
                <p>Get guidance and support from experienced developers and mentors.</p>
            </div>
        </div>
    </section>
    
    <!-- success stories Section -->
    <section id="success-stories" class="success-stories">
        <h2>Success Stories</h2>
        <div class="stories-container">
            <div class="story-card">
                <h3>Emily R.</h3>
                <p>"Thanks to Coding Hub, I landed my first job as a software engineer at a top company!"</p>
            </div>
            <div class="story-card">
                <h3>Michael T.</h3>
                <p>"The real-world projects and interactive lessons helped me level up my skills quickly."</p>
            </div>
            <div class="story-card">
                <h3>Sophia L.</h3>
                <p>"Coding Hub made learning coding fun and effective. Highly recommend for beginners!"</p>
            </div>
        </div>
    </section>
    

     <!-- Testimonials Section -->
     <section class="testimonial">
        <h2>What Our Users Say</h2>
        <div>
            <h3 style="text-align: center;">John Doe</h3>
            <p>"Coding Hub transformed my coding journey. The interactive lessons and challenges made it fun and easy to learn."</p>
        </div>
    </section>

    <!-- Footer Section -->
    <footer>
        
        <div class="social-links">
            <a href="#">Facebook</a>
            <a href="#">Twitter</a>
            <a href="#">LinkedIn</a>
        </div>
        <p>&copy; 2024 Coding Hub. All rights reserved.</p>
    </footer>
</body>
</html>
