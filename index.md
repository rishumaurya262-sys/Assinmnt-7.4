# Assignment 7.4 — Modern Landing Page Header

## HTML Code (`index.html`)

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Modern Landing Page</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <header class="header">
        <a href="#" class="logo">NovaTech</a>

        <nav class="nav-links">
            <a href="#">Home</a>
            <a href="#">Features</a>
            <a href="#">About</a>
            <a href="#">Contact</a>
        </nav>

        <a href="#" class="cta-button">Get Started</a>
    </header>

    <main>
        <section class="hero">
            <div class="hero-content">
                <h1>Build Your Future with NovaTech</h1>
                <p>
                    Discover modern solutions that help you work smarter,
                    grow faster, and achieve your goals.
                </p>
                <a href="#" class="hero-button">Explore Now</a>
            </div>

            <div class="hero-image">
                <img
                    src="https://placehold.co/600x400?text=Modern+Technology"
                    alt="Modern technology illustration"
                >
            </div>
        </section>
    </main>

    <footer class="footer">
        <p>© 2026 NovaTech. All rights reserved.</p>
    </footer>
</body>
</html>
```

## CSS Code (`style.css`)

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    color: #1e293b;
    background-color: #f8fafc;
}

.header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 20px 6%;
    background-color: white;
    gap: 20px;
    flex-wrap: wrap;
}

.logo {
    font-size: 26px;
    font-weight: bold;
    color: #2563eb;
    text-decoration: none;
}

.nav-links {
    display: flex;
    align-items: center;
    gap: 25px;
}

.nav-links a {
    color: #334155;
    text-decoration: none;
}

.nav-links a:hover {
    color: #2563eb;
}

.cta-button,
.hero-button {
    display: inline-block;
    padding: 12px 20px;
    background-color: #2563eb;
    color: white;
    text-decoration: none;
    border-radius: 6px;
}

.cta-button:hover,
.hero-button:hover {
    background-color: #1d4ed8;
}

.hero {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 40px;
    padding: 70px 6%;
    min-height: 500px;
}

.hero-content {
    flex: 1;
}

.hero-content h1 {
    font-size: 42px;
    line-height: 1.2;
    margin-bottom: 20px;
}

.hero-content p {
    font-size: 18px;
    line-height: 1.7;
    color: #64748b;
    margin-bottom: 25px;
}

.hero-image {
    flex: 1;
}

.hero-image img {
    width: 100%;
    height: auto;
    display: block;
    border-radius: 12px;
}

.footer {
    text-align: center;
    padding: 20px;
    background-color: #1e293b;
    color: white;
}

@media (max-width: 700px) {
    .header {
        flex-direction: column;
    }

    .nav-links {
        justify-content: center;
        flex-wrap: wrap;
        gap: 15px;
    }

    .hero {
        flex-direction: column;
        text-align: center;
        padding: 45px 6%;
    }

    .hero-content h1 {
        font-size: 32px;
    }
}
```

## Result

A modern, responsive landing page was created using HTML and CSS. The header contains a logo, navigation links, and a call-to-action button. The hero section includes a heading, paragraph, button, and image arranged side-by-side using Flexbox. The footer is styled, and a media query adjusts the layout for smaller screens.

## Testing

Open `index.html` using Live Server. Check the page at desktop and mobile widths to verify that the header and hero section remain properly aligned.