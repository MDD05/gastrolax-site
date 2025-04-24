# gastrolax-site
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GASTRO LAX | Dual Action Syrup</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <!-- Header & Logo -->
    <header>
        <img src="images/logo.png" alt="GASTRO LAX Logo" class="logo">
        <img src="qr-code.png" alt="QR Code" class="qr-code">
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <img src="images/bottle.jpg" alt="GASTRO LAX Bottle">
        <h1>Fast Relief for Acidity & Constipation</h1>
        <p>Dual Action Syrup – Neutralizes Acid, Eases Digestion.</p>
    </section>

    <!-- Key Benefits -->
    <section class="benefits">
        <div class="card">
            💊 <h3>Neutralizes Acid</h3>
            <p>Quickly relieves heartburn and indigestion.</p>
        </div>
        <div class="card">
            🌿 <h3>Gentle Laxative</h3>
            <p>Promotes comfortable bowel movements.</p>
        </div>
        <div class="card">
            ⭐ <h3>Pleasant & Sugar-Free</h3>
            <p>Refreshing mint taste.</p>
        </div>
    </section>

    <!-- Rewards Section -->
    <section class="rewards">
        <h2>Earn Points with Every Purchase</h2>
        <ul>
            <li>Buy 1 bottle = 10 points</li>
            <li>50 points = Free Shipping</li>
            <li>100 points = Free Bottle</li>
        </ul>
    </section>

    <!-- Footer -->
    <footer>
        <p>Consult your doctor before use. Manufactured by GASTRO LAX Team × Gallala University.</p>
    </footer>
</body>
</html>
body {
    font-family: Arial, sans-serif;
    margin: 0;
    background: #F8F9FA;
}

.logo {
    width: 200px;
    margin: 20px;
}

.qr-code {
    width: 100px;
    position: absolute;
    top: 20px;
    right: 20px;
}

.hero {
    text-align: center;
    padding: 50px;
    background: #2A5C8F;
    color: white;
}

.hero img {
    width: 300px;
}

.benefits {
    display: flex;
    justify-content: center;
    gap: 20px;
    padding: 40px;
}

.card {
    background: white;
    padding: 20px;
    border-radius: 10px;
    width: 250px;
    text-align: center;
}

.rewards {
    background: #8BC34A;
    padding: 30px;
    text-align: center;
}

footer {
    background: #2A5C8F;
    color: white;
    text-align: center;
    padding: 20px;
}
