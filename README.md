<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Landing Page</title>
    <style>
        /* Navigation menu styles */
       .nav {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: #333;
            padding: 1rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
            z-index: 1000;
        }

       .nav ul {
            list-style: none;
            margin: 0;
            padding: 0;
            display: flex;
        }

       .nav li {
            margin-right: 20px;
        }

       .nav a {
            color: #fff;
            text-decoration: none;
            transition: color 0.2s ease;
        }

       .nav a:hover {
            color: #ccc;
        }

        /* Scroll effect */
       .nav.scrolled {
            background-color: #444;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.2);
        }

        /* Hover effect */
       .nav li:hover > a {
            color: #fff;
            background-color: #666;
            padding: 10px 20px;
            border-radius: 10px;
        }

        /* Responsive styles */
        @media (max-width: 768px) {
           .nav {
                flex-direction: column;
                align-items: flex-start;
            }
           .nav ul {
                flex-direction: column;
            }
           .nav li {
                margin-right: 0;
            }
           .nav a {
                padding: 10px 20px;
            }
        }
    </style>
</head>
<body>
    <nav class="nav">
        <ul>
            <li><a href="#home">Home</a></li>
            <li><a href="#about">About</a></li>
            <li><a href="#services">Services</a></li>
            <li><a href="#contact">Contact</a></li>
        </ul>
    </nav>
    <main>
        <section id="home">
            <h1>Welcome to our landing page</h1>
            <p>Greetings and welcome to our landing page! We are delighted to see you as a part of our community. Feel free to discover, interact, and collaborate with us to create something wonderful</p>
        </section>
        <section id="about">
            <h1>About us</h1>
            <p>Hello,My self Abhishek shukla and I am pursuig my graduation(BCA) from United Univesity Jhalwa Prayagraj. </p>
        </section>
        <section id="services">
            <h1>Our services</h1>
            <p>This landing page promotes a company that helps new music artists to create their brand and produce and license their music.</p>
        </section>
        <section id="contact">
            <h1>Get in touch</h1>
            <p>We can ensure reliability, low cost fares and most important, with safety and comfort in mind.</p>
        </section>
    </main>
    <script>
        // Add event listener to window scroll event
        window.addEventListener('scroll', function() {
            // Get the navigation menu element
            const nav = document.querySelector('.nav');

            // Check if the user has scrolled down
            if (window.scrollY > 200) {
                // Add the scrolled class to the navigation menu
                nav.classList.add('scrolled');
            } else {
                // Remove the scrolled class from the navigation menu
                nav.classList.remove('scrolled');
            }
        });
    </script>
</body>
</html>
