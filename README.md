# gastrolax-site
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>GASTRO LAX® - Official Portal</title>
    <style>
        :root {
            --primary-blue: #2A5C8F;
            --mint-green: #8BC34A;
            --warning-red: #D32F2F;
            --neutral-white: #FFFFFF;
            --background-gray: #F8F9FA;
        }

        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            background: var(--background-gray);
            color: #333;
            line-height: 1.7;
        }

        .product-header {
            background: linear-gradient(135deg, var(--primary-blue) 60%, var(--mint-green));
            padding: 2rem 1rem;
            text-align: center;
            color: var(--neutral-white);
            box-shadow: 0 4px 15px rgba(0,0,0,0.1);
        }

        .product-visual {
            max-width: 800px;
            margin: 2rem auto;
            padding: 1rem;
            background: var(--neutral-white);
            border-radius: 12px;
            border: 2px solid var(--primary-blue);
        }

        .medical-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 2rem auto;
            padding: 1rem;
        }

        .warning {
            background: #FFEBEE;
            border-left: 4px solid var(--warning-red);
            padding: 1.5rem;
            margin: 1rem 0;
        }

        .qr-section {
            text-align: center;
            padding: 2rem;
            background: var(--mint-green);
            margin: 2rem auto;
            max-width: 600px;
            border-radius: 12px;
        }

        .fab {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: var(--primary-blue);
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            cursor: pointer;
            box-shadow: 0 4px 12px rgba(0,0,0,0.2);
            z-index: 1000;
        }

        @media (max-width: 768px) {
            .medical-grid {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <!-- Product Header -->
    <header class="product-header">
        <h1>GASTRO LAX®</h1>
        <h2>DUAL ACTION SYRUP</h2>
        <p>Antacid + Gentle Laxative Formula</p>
    </header>

    <!-- Main Product Image -->
    <div class="product-visual">
        <img src="https://i.ibb.co/KxMW0w7Q/IMG-0290.jpg" 
             alt="GASTRO LAX Product Label" 
             style="width:100%; border-radius:8px;">
    </div>

    <!-- Comprehensive Product Information -->
    <div class="medical-grid">
        <!-- Left Column -->
        <div>
            <h3>Key Benefits</h3>
            <ul>
                <li>⚡ Fast-acting formula (30-60 minute relief)</li>
                <li>⚖️ Dual action: Neutralizes acid + promotes digestion</li>
                <li>🌿 Natural peppermint flavor</li>
                <li>📏 Precision dosing for adults & children 12+</li>
            </ul>

            <h3>Pharmacological Properties</h3>
            <ul>
                <li>🕒 Onset of Action: 30-45 minutes</li>
                <li>⏳ Duration of Effect: 4-6 hours</li>
                <li>🧪 pH Neutralization Capacity: 12.5 mEq/10ml</li>
                <li>📈 Bioavailability: 85-90%</li>
            </ul>

            <div class="warning">
                <h3>Important Warnings</h3>
                <ul>
                    <li>❌ Not for long-term use (>7 days)</li>
                    <li>❌ Avoid if kidney disease present</li>
                    <li>❌ Keep out of children's reach</li>
                </ul>
            </div>
        </div>

        <!-- Right Column -->
        <div>
            <h3>Usage Instructions</h3>
            <table style="width:100%">
                <tr>
                    <th>Age Group</th>
                    <th>Dosage</th>
                    <th>Frequency</th>
                </tr>
                <tr>
                    <td>Adults</td>
                    <td>10-15 ml</td>
                    <td>3× daily</td>
                </tr>
                <tr>
                    <td>Teens 12-17</td>
                    <td>5-10 ml</td>
                    <td>2× daily</td>
                </tr>
            </table>

            <h3>Active Ingredients</h3>
            <ul>
                <li>Magnesium sulfate (480mg/10ml)</li>
                <li>Light magnesium carbonate (320mg/10ml)</li>
                <li>Peppermint oil extract (0.5ml/10ml)</li>
            </ul>

            <div class="warning">
                <h3>Storage & Handling</h3>
                <ul>
                    <li>Store at 15-25°C (59-77°F)</li>
                    <li>Protect from direct sunlight</li>
                    <li>Use within 28 days of opening</li>
                </ul>
            </div>
        </div>
    </div>

    <!-- QR & Rewards Section -->
    <div class="qr-section">
        <h2>Rewards Program</h2>
        <img src="https://api.qrserver.com/v1/create-qr-code/?data=https://gastrolax.com/rewards&size=150x150&color=2A5C8F" 
             alt="Rewards QR Code">
        <div style="margin-top: 1rem;">
            <h3>Earn Points with Every Purchase</h3>
            <ul style="text-align: left; display: inline-block;">
                <li>• 1 bottle = 10 points</li>
                <li>• 50 points = Free shipping</li>
                <li>• 100 points = Free product</li>
            </ul>
        </div>
    </div>

    <!-- Second Product Image -->
    <div class="product-visual" style="max-width:600px;">
        <img src="https://i.ibb.co/svTLrCb8/IMG-0297.jpg" 
             alt="Additional Product Info" 
             style="width:100%; border-radius:8px;">
    </div>

    <!-- Floating Action Button -->
    <div class="fab" onclick="toggleMenu()">⚙️</div>

    <!-- Settings Menu -->
    <div id="settingsMenu" style="display:none; position:fixed; bottom:100px; right:30px; background:white; padding:1rem; border-radius:8px; box-shadow:0 4px 12px rgba(0,0,0,0.2);">
        <h3>User Settings</h3>
        <button onclick="showLogin()">Login</button>
        <button onclick="showPreferences()">Preferences</button>
    </div>

    <!-- Footer -->
    <footer style="background:var(--primary-blue); color:white; text-align:center; padding:2rem; margin-top:3rem;">
        <p>Manufactured by GASTRO LAX Pharmaceuticals<br>
        Certified by Gallala University Medical Board<br>
        Distributed under license in Pennsylvania</p>
        <p style="margin-top:1rem;"><small>Always consult your physician before use</small></p>
    </footer>

    <script>
        // Settings Menu Functions
        function toggleMenu() {
            const menu = document.getElementById('settingsMenu');
            menu.style.display = menu.style.display === 'block' ? 'none' : 'block';
        }

        function showLogin() {
            alert('Login functionality would appear here');
        }

        function showPreferences() {
            alert('User preferences panel would appear here');
        }
    </script>
</body>
</html>
