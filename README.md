
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Travel and Tour</title>
    <link rel="stylesheet" href="styles.css">
</head>
<body>
    <header>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#packages">Packages</a></li>
                <li><a href="#destinations">Destinations</a></li>
                <li><a href="#contact">Contact</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <section id="home">
            <h1>Welcome to Travel and Tour</h1>
            <p>Explore the world with us!</p>
            <button>Book Now</button>
        </section>
        <section id="packages">
            <h2>Our Packages</h2>
            <div class="package-container">
                <div class="package">
                    <h3>Package 1</h3>
                    <p>3 Days, 2 Nights</p>
                    <p>Price: $500</p>
                </div>
                <div class="package">
                    <h3>Package 2</h3>
                    <p>5 Days, 4 Nights</p>
                    <p>Price: $1000</p>
                </div>
                <!-- Add more packages -->
            </div>
        </section>
        <section id="destinations">
            <h2>Our Destinations</h2>
            <div class="destination-container">
                <div class="destination">
                    <h3>Paris</h3>
                    <p>France</p>
                </div>
                <div class="destination">
                    <h3>Rome</h3>
                    <p>Italy</p>
                </div>
                <!-- Add more destinations -->
            </div>
        </section>
        <section id="contact">
            <h2>Get in Touch</h2>
            <form>
                <input type="text" placeholder="Name">
                <input type="email" placeholder="Email">
                <textarea placeholder="Message"></textarea>
                <button>Send</button>
            </form>
        </section>
    </main>
    <script src="script.js"></script>
</body>
</html>
```

*CSS (styles.css)*
```
body {
    font-family: Arial, sans-serif;
    margin: 0;
    padding: 0;
}

header {
    background-color: #333;
    color: #fff;
    padding: 1em;
    text-align: center;
}

nav ul {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: space-between;
}

nav li {
    margin-right: 20px;
}

nav a {
    color: #fff;
    text-decoration: none;
}

main {
    display: flex;
    flex-direction: column;
    align-items: center;
    padding: 2em;
}

section {
    background-color: #f7f7f7;
    padding: 2em;
    margin-bottom: 20px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

h1, h2, h3 {
    color: #333;
    margin-bottom: 10px;
}

.package-container, .destination-container {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}

.package, .destination {
    background-color: #fff;
    padding: 1em;
    margin: 10px;
    width: calc(33.33% - 20px);
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}

button {
    background-color: #333;
    color: #fff;
    border: none;
    padding: 10px 20px;
    font-size: 16px;
    cursor: pointer;
}

button:hover {
    background-color: #555;
}
```

*JavaScript (script.js)*
```
// Add event listener to book now button
document.querySelector('button').addEventListener('click', () => {
    alert('Booking successful!');
});

// Add event listener to package selection
const packages = document.querySelectorAll('.package');
packages.forEach((package) => {
    package.addEventListener('click', () => {
        const packageName = package.querySelector('h3').textContent;
        alert
```
