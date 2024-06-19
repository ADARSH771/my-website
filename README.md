# my-website
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Software Company</title>
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            background-color: #f0f2f5;
            color: #333;
        }

        header {
            background-color: #2C3E50;
            padding: 15px 0;
            box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
        }

        nav ul {
            list-style: none;
            display: flex;
            justify-content: center;
            margin: 0;
            padding: 0;
        }

        nav ul li {
            margin: 0 20px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            font-size: 1.2em;
        }

        nav ul li a:hover {
            color: #18bc9c;
            transition: color 0.3s;
        }

        .hero-section {
            background: linear-gradient(135deg, #2980B9 0%, #6DD5FA 100%);
            color: white;
            text-align: center;
            padding: 120px 20px;
        }

        .hero-section h1 {
            margin: 0;
            font-size: 3.5em;
        }

        .hero-section p {
            font-size: 1.5em;
            margin: 20px 0;
        }

        .hero-section button {
            background-color: #18bc9c;
            color: white;
            border: none;
            padding: 15px 30px;
            font-size: 1.2em;
            cursor: pointer;
            border-radius: 5px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        .hero-section button:hover {
            background-color: #16a085;
            transition: background-color 0.3s;
        }

        .services-section, .team-section, .pricing-section, .testimonials-section, .faq-section, .contact-section {
            text-align: center;
            padding: 60px 20px;
        }

        .services-section h2, .team-section h2, .pricing-section h2, .testimonials-section h2, .faq-section h2, .contact-section h2 {
            font-size: 2.5em;
            margin-bottom: 40px;
            color: #2C3E50;
        }

        .service-card, .team-member, .testimonial, .faq-item {
            background-color: white;
            margin: 20px;
            padding: 30px;
            border-radius: 10px;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
            transition: transform 0.3s, box-shadow 0.3s;
        }

        .service-card:hover, .team-member:hover, .testimonial:hover, .faq-item:hover {
            transform: translateY(-10px);
            box-shadow: 0 6px 20px rgba(0, 0, 0, 0.2);
        }

        .service-card h3, .team-member h3, .testimonial h3, .faq-item h3 {
            color: #18bc9c;
            margin-bottom: 15px;
        }

        .service-card p, .team-member p, .testimonial p, .faq-item p {
            color: #7f8c8d;
        }

        .team-member img {
            border-radius: 15px;
            width: 150px;
            height: 200px;
            margin-bottom: 15px;
            object-fit: cover;
            border: 5px solid #18bc9c;
        }

        table {
            width: 100%;
            max-width: 800px;
            margin: 0 auto;
            border-collapse: collapse;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
        }

        table thead {
            background-color: #18bc9c;
            color: white;
        }

        table th, table td {
            padding: 15px;
            border: 1px solid #ddd;
            text-align: center;
        }

        table tbody tr:nth-child(odd) {
            background-color: #f9f9f9;
        }

        form {
            display: flex;
            flex-direction: column;
            align-items: center;
        }

        form label {
            font-weight: bold;
            margin-top: 10px;
            color: #2C3E50;
        }

        form input, form textarea {
            width: 100%;
            max-width: 500px;
            padding: 10px;
            margin-top: 5px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }

        form button {
            background-color: #18bc9c;
            color: white;
            border: none;
            padding: 15px 30px;
            margin-top: 20px;
            cursor: pointer;
            border-radius: 5px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
        }

        form button:hover {
            background-color: #16a085;
            transition: background-color 0.3s;
        }

        footer {
            background-color: #2C3E50;
            color: white;
            text-align: center;
            padding: 20px 0;
            box-shadow: 0 -2px 4px rgba(0, 0, 0, 0.1);
        }
    </style>
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#services">Services</a></li>
                <li><a href="#team">Team</a></li>
                <li><a href="#pricing">Pricing</a></li>
                <li><a href="#testimonials">Testimonials</a></li>
                <li><a href="#faq">FAQ</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>

    <section id="home" class="hero-section">
        <h1>Welcome to Our Software Company</h1>
        <p>Delivering innovative software solutions to help your business grow.</p>
        <button onclick="learnMore()">Learn More</button>
    </section>

    <section id="services" class="services-section">
        <h2>Our Services</h2>
        <div class="service-card">
            <h3>Web Development</h3>
            <p>Building responsive and modern websites.</p>
        </div>
        <div class="service-card">
            <h3>Mobile Development</h3>
            <p>Creating mobile apps for iOS and Android.</p>
        </div>
        <div class="service-card">
            <h3>Cloud Solutions</h3>
            <p>Offering scalable cloud solutions for your business.</p>
        </div>
    </section>

    <section id="team" class="team-section">
        <h2>Meet Our Team</h2>
        <div class="team-member">
            <img src="member1.jpg" alt="Team Member 1">
            <h3>John Doe</h3>
            <p>CEO</p>
        </div>
        <div class="team-member">
            <img src="member2.jpg" alt="Team Member 2">
            <h3>Jane Smith</h3>
            <p>CTO</p>
        </div>
        <div class="team-member">
            <img src="member3.jpg" alt="Team Member 3">
            <h3>Mike Johnson</h3>
            <p>Lead Developer</p>
        </div>
    </section>

    <section id="pricing" class="pricing-section">
        <h2>Pricing Plans</h2>
        <table>
            <thead>
                <tr>
                    <th>Plan</th>
                    <th>Features</th>
                    <th>Price</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Basic</td>
                    <td>Web Development, Support</td>
                    <td>$100/month</td>
                </tr>
                <tr>
                    <td>Standard</td>
                    <td>Web & Mobile Development, Cloud Solutions</td>
                    <td>$200/month</td>
                </tr>
                <tr>
                    <td>Premium</td>
                    <td>All Services, 24/7 Support</td>
                    <td>$500/month</td>
                </tr>
            </tbody>
        </table>
    </section>

    <section id="testimonials" class="testimonials-section">
        <h2>What Our Clients Say</h2>
        <div class="testimonial">
            <p>"The team was professional and efficient. Highly recommend their services!"</p>
            <h3>- Sarah Williams</h3>
        </div>
        <div class="testimonial">
            <p>"Our project was completed on time and exceeded our expectations. Excellent work!"</p>
            <h3>- David Brown</h3>
        </div>
    </section>

    <section id="faq" class="faq-section">
        <h2>Frequently Asked Questions</h2>
        <div class="faq-item">
            <h3>What services do you offer?</h3>
            <p>We offer web development, mobile app development, and cloud solutions.</p>
        </div>
        <div class="faq-item">
            <h3>What is your pricing structure?</h3>
            <p>We offer three plans: Basic, Standard, and Premium. Details are available in the pricing section.</p>
        </div>
        <div class="faq-item">
            <h3>How can we contact you?</h3>
            <p>You can reach us via the contact form below or at contact@softwarecompany.com.</p>
        </div>
    </section>

    <section id="contact" class="contact-section">
        <h2>Contact Us</h2>
        <form action="submit-form.php" method="post">
            <label for="name">Name:</label>
            <input type="text" id="name" name="name" required>
            
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            
            <label for="message">Message:</label>
            <textarea id="message" name="message" required></textarea>
            
            <button type="submit">Submit</button>
        </form>
    </section>

    <footer>
        <p>&copy; 2024 Software Company. All rights reserved.</p>
    </footer>

    <script>
        function learnMore() {
            window.location.href = "#services";
        }
    </script>
</body>
</html>
