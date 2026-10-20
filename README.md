
# Experiment 6 – Simple Website Using HTML, CSS and JavaScript

## a1.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
    <title>My Simple Website</title>
    <link rel="stylesheet" href="style.css" />
</head>
<body onload="welcomeUser()">

    <header>
        <h1>Welcome to My Website</h1>
        <nav>
            <a href="#home">Home</a>
            <a href="#about">About</a>
            <a href="#services">Services</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <main>
        <section id="home">
            <h2>Home</h2>
            <p>This is the homepage section.</p>
        </section>

        <section id="about">
            <h2>About This Site</h2>
            <p>This is a beginner-friendly website made using HTML, CSS, and JavaScript.</p>
            <button onclick="showMessage()">Click Me!</button>
            <p id="message"></p>
        </section>

        <section id="services">
            <h2>Our Services</h2>
            <ul>
                <li>Web Design</li>
                <li>App Development</li>
                <li>JavaScript Training</li>
            </ul>
        </section>

        <section id="contact">
            <h2>Contact Us</h2>
            <p>Email: example@mywebsite.com</p>
            <p>Phone: 123-456-7890</p>
        </section>
    </main>

    <footer>
        <p>&copy; 2025 MyWebsite. All rights reserved.</p>
    </footer>

    <script src="script.js"></script>
</body>
</html>
```

## style.css

```css
html {
    scroll-behavior: smooth;
}

body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
    background-color: #f8f9fa;
}

header {
    background-color: #0077cc;
    color: white;
    padding: 20px;
    text-align: center;
}

nav a {
    color: white;
    margin: 10px;
    text-decoration: none;
    font-weight: bold;
}

nav a:hover {
    text-decoration: underline;
}

section {
    padding: 40px;
    background-color: white;
    border-bottom: 1px solid #ddd;
}

footer {
    background-color: #333;
    color: white;
    text-align: center;
    padding: 15px;
}

button {
    background-color: #0077cc;
    color: white;
    padding: 10px 15px;
    border: none;
    cursor: pointer;
    font-size: 16px;
    border-radius: 5px;
    margin-top: 10px;
}

button:hover {
    background-color: #005fa3;
}

#message {
    color: green;
    font-weight: bold;
    margin-top: 10px;
}
```

## script.js

```javascript
function welcomeUser() {
    alert("Welcome to our website!");
}

function showMessage() {
    const message = document.getElementById("message");
    message.textContent = "Thank you for clicking! Enjoy browsing";
}
```
