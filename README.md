<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Custom Color Website</title>
    <style>
        body {
            background-color: #F8FBFF;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            padding: 20px;
            margin: 0;
        }

        h1 {
            color: #0077B6;
            text-align: center;
            font-size: 48px;
            margin-bottom: 30px;
            text-shadow: 0 2px 10px rgba(0, 119, 182, 0.2);
        }

        h2 {
            color: #0077B6;
            font-size: 36px;
            margin-top: 30px;
        }

        h3 {
            color: #00B4D8;
            font-size: 28px;
        }

        h4 {
            color: #0077B6;
            font-size: 20px;
            margin: 0 0 10px 0;
        }

        p {
            color: #023047;
            font-size: 18px;
            line-height: 1.8;
        }

        .container {
            max-width: 900px;
            margin: 0 auto;
        }

        .box {
            background-color: #EAF4FF;
            padding: 25px;
            margin: 20px 0;
            border-radius: 15px;
            border-left: 5px solid #0077B6;
            box-shadow: 0 4px 12px rgba(0, 119, 182, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .box:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 119, 182, 0.2);
        }

        .box-secondary {
            background-color: #EAF4FF;
            color: #023047;
            padding: 25px;
            margin: 20px 0;
            border-radius: 15px;
            border-left: 5px solid #00B4D8;
            box-shadow: 0 4px 12px rgba(0, 180, 216, 0.1);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }

        .box-secondary:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 20px rgba(0, 180, 216, 0.2);
        }

        .box-success {
            background-color: #EAF4FF;
            color: #023047;
            padding: 25px;
            margin: 20px 0;
            border-radius: 15px;
            border-left: 5px solid #2ECC71;
            box-shadow: 0 4px 12px rgba(46, 204, 113, 0.1);
        }

        .box-warning {
            background-color: #EAF4FF;
            color: #023047;
            padding: 25px;
            margin: 20px 0;
            border-radius: 15px;
            border-left: 5px solid #F4A261;
            box-shadow: 0 4px 12px rgba(244, 162, 97, 0.1);
        }

        .feature {
            background-color: #F8FBFF;
            padding: 15px;
            margin: 15px 0;
            border-radius: 10px;
            border-left: 4px solid #00B4D8;
            border: 1px solid #00B4D8;
        }

        .feature h4 {
            color: #0077B6;
        }

        .feature p {
            color: #023047;
            margin: 0;
        }

        .badge {
            display: inline-block;
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 14px;
            font-weight: bold;
            margin-right: 10px;
            margin-bottom: 10px;
        }

        .badge-primary {
            background-color: #0077B6;
            color: white;
        }

        .badge-secondary {
            background-color: #00B4D8;
            color: white;
        }

        .badge-success {
            background-color: #2ECC71;
            color: white;
        }

        .badge-warning {
            background-color: #F4A261;
            color: white;
        }

        .badge-danger {
            background-color: #D62828;
            color: white;
        }

        .highlight {
            color: #00B4D8;
            font-weight: bold;
        }

        button {
            background-color: #0077B6;
            color: white;
            border: none;
            padding: 12px 24px;
            font-size: 16px;
            border-radius: 8px;
            cursor: pointer;
            margin-top: 15px;
            transition: background-color 0.3s ease;
        }

        button:hover {
            background-color: #005a8d;
        }

        .button-secondary {
            background-color: #00B4D8;
        }

        .button-secondary:hover {
            background-color: #0099ba;
        }

        /* Health Score Form Styles */
        .form-container {
            background-color: white;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }

        .health-score-box {
            background-color: #EAF4FF;
            padding: 25px;
            margin: 20px 0;
            border-radius: 15px;
            border-left: 5px solid #0077B6;
            box-shadow: 0 4px 12px rgba(0, 119, 182, 0.1);
        }

        .health-score-box h2 {
            color: #0077B6;
            font-size: 36px;
            margin-top: 0;
            margin-bottom: 20px;
            text-align: center;
        }

        .form-group {
            margin-bottom: 20px;
        }

        .form-group label {
            display: block;
            margin-bottom: 5px;
            color: #023047;
            font-weight: bold;
            font-size: 16px;
        }

        .form-group input {
            width: 100%;
            padding: 10px;
            border: 2px solid #00B4D8;
            border-radius: 4px;
            box-sizing: border-box;
            font-size: 14px;
            transition: border-color 0.3s ease;
        }

        .form-group input:focus {
            outline: none;
            border-color: #0077B6;
            background-color: #f9f9f9;
        }

        .form-group input::placeholder {
            color: #999;
        }

        .health-form-button {
            width: 100%;
            padding: 12px;
            background-color: #0077B6;
            color: white;
            border: none;
            border-radius: 4px;
            font-size: 16px;
            font-weight: bold;
            cursor: pointer;
            transition: background-color 0.3s ease;
            margin-top: 0;
        }

        .health-form-button:hover {
            background-color: #005a8d;
        }

        .result {
            margin-top: 30px;
            padding: 20px;
            background-color: #F0F0F0;
            border-radius: 4px;
            display: none;
            border-left: 5px solid #00B4D8;
        }

        .result.show {
            display: block;
        }

        .result h3 {
            color: #0077B6;
            margin-top: 0;
        }

        .result p {
            color: #023047;
            margin: 10px 0;
        }

        .bmi-value {
            font-size: 32px;
            font-weight: bold;
            color: #4CAF50;
            text-align: center;
            margin: 15px 0;
        }

        .bmi-category {
            text-align: center;
            font-size: 18px;
            color: #555;
            font-weight: bold;
            margin: 10px 0;
        }

        /* BMI Chart Styles */
        .bmi-chart {
            margin-top: 30px;
            border-collapse: collapse;
            width: 100%;
            background-color: white;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
            border-radius: 8px;
            overflow: hidden;
        }

        .bmi-chart th {
            background-color: #0077B6;
            color: white;
            padding: 15px;
            text-align: left;
            font-size: 16px;
            font-weight: bold;
        }

        .bmi-chart td {
            padding: 15px;
            border-bottom: 1px solid #ddd;
            color: #023047;
            font-size: 15px;
        }

        .bmi-chart tr:last-child td {
            border-bottom: none;
        }

        .bmi-chart tr:hover {
            background-color: #f5f5f5;
        }

        .chart-title {
            text-align: center;
            color: #0077B6;
            font-size: 24px;
            font-weight: bold;
            margin-bottom: 20px;
            margin-top: 30px;
        }

        .underweight-row {
            border-left: 5px solid #2196F3;
        }

        .normal-row {
            border-left: 5px solid #4CAF50;
        }

        .overweight-row {
            border-left: 5px solid #FF9800;
        }

        .obesity-row {
            border-left: 5px solid #F44336;
        }

        .result-container {
            display: flex;
            justify-content: center;
            align-items: center;
            margin: 20px 0;
            flex-wrap: wrap;
        }

        .bmi-indicator {
            width: 100px;
            height: 100px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 32px;
            font-weight: bold;
            color: white;
            margin: 10px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.2);
        }

        .indicator-text {
            margin-left: 20px;
            text-align: left;
        }

        .indicator-text p {
            margin: 5px 0;
        }
    </style>
</head>
<body>

    <div class="container">
        <h1>Welcome to Vospk</h1>

        <div class="box">
            <h2>About Us</h2>
            <p>At our core, we are dedicated to empowering individuals with smarter, data-driven health insights. Our disease prediction platform uses advanced algorithms and intelligent analysis to assess symptoms, lifestyle factors, and health indicators to provide personalized risk evaluations. Beyond prediction, our website offers tailored health recommendations, practical wellness advice, and an easy-to-understand health score that reflects your overall well-being. We believe that preventive care starts with awareness, and our mission is to make reliable health guidance accessible, simple, and actionable for everyone. By combining technology with health expertise, we aim to help you make informed decisions and take proactive steps toward a healthier future.</p>
            <button>Learn More</button>
        </div>

        <!-- Health Score Form Section -->
        <div class="health-score-box">
            <h2>Health Score  📈 </h2>
            <div class="form-container">
                <form id="healthScoreForm">
                    <!-- Weight Section -->
                    <div class="form-group">
                        <label for="weight">Weight (kg):</label>
                        <input type="number" id="weight" name="weight" step="0.1" required placeholder="Enter your weight">
                    </div>
                    
                    <!-- Height Section -->
                    <div class="form-group">
                        <label for="height">Height (m):</label>
                        <input type="number" id="height" name="height" step="0.01" required placeholder="Enter your height (e.g., 1.75)">
                    </div>
                    
                    <!-- Date of Birth Section -->
                    <div class="form-group">
                        <label for="dob">Date of Birth:</label>
                        <input type="date" id="dob" name="dob" required>
                    </div>
                    
                    <!-- Submit Button -->
                    <button type="submit" class="health-form-button">Calculate BMI</button>
                </form>
                
                <!-- Results Section -->
                <div id="result" class="result">
                    <h3>Your Health Score</h3>
                    <p><strong>Age:</strong> <span id="age"></span> years</p>
                    
                    <div class="result-container">
                        <div class="bmi-indicator" id="bmiIndicator"></div>
                        <div class="indicator-text">
                            <p><strong>BMI Value:</strong> <span id="bmiValue" style="font-size: 24px;"></span></p>
                            <p><strong>Status:</strong> <span id="bmiCategory" style="font-size: 18px;"></span></p>
                        </div>
                    </div>
                </div>

                <!-- BMI Chart Reference -->
                <div class="chart-title">BMI Reference Chart</div>
                <table class="bmi-chart">
                    <thead>
                        <tr>
                            <th>BMI Range</th>
                            <th>Weight Status</th>
                        </tr>
                    </thead>
                    <tbody>
                        <tr class="underweight-row">
                            <td><strong>Below 18.5</strong></td>
                            <td>Underweight</td>
                        </tr>
                        <tr class="normal-row">
                            <td><strong>18.5 - 24.9</strong></td>
                            <td>Normal weight</td>
                        </tr>
                        <tr class="overweight-row">
                            <td><strong>25.0 - 29.9</strong></td>
                            <td>Overweight</td>
                        </tr>
                        <tr class="obesity-row">
                            <td><strong>30.0 and above</strong></td>
                            <td>Obesity</td>
                        </tr>
                    </tbody>
                </table>
            </div>
        </div>

        <div class="box-secondary">
            <h2>🎯 Our Services</h2>
            <div class="feature">
                <h4>✨ Web Design</h4>
                <p>Beautiful, modern designs that capture your brand's essence and engage your audience.</p>
            </div>
            <div class="feature">
                <h4>🚀 Web Development</h4>
                <p>Fast, responsive, and reliable websites built with the latest technology and best practices.</p>
            </div>
            <div class="feature">
                <h4>💡 Creative Solutions</h4>
                <p>Innovative ideas tailored to your unique business needs and goals.</p>
            </div>
            <div class="feature">
                <h4>📱 Mobile First</h4>
                <p>Perfectly optimized for all devices - phones, tablets, and desktops.</p>
            </div>
        </div>

        <div class="box-success">
            <h2>✓ Why Choose Us?</h2>
            <p>Our team brings years of experience in creating <span class="highlight">professional websites</span> that deliver results. We focus on quality, performance, and user experience to ensure your online presence stands out from the competition.</p>
            <div>
                <span class="badge badge-success">Quality Assured</span>
                <span class="badge badge-success">Fast Delivery</span>
                <span class="badge badge-success">Expert Team</span>
            </div>
        </div>

        <div class="box-warning">
            <h2>⚠️ Special Offers</h2>
            <p>Limited time! Get 20% off on all web design packages this month. Don't miss this opportunity to elevate your online presence with our professional services.</p>
            <button class="button-secondary">Claim Offer</button>
        </div>

        <div class="box">
            <h2>📊 Our Features</h2>
            <div style="margin: 20px 0;">
                <p><span class="badge badge-primary">Primary Color</span> - Main branding and CTAs</p>
                <p><span class="badge badge-secondary">Secondary Color</span> - Highlights and accents</p>
                <p><span class="badge badge-success">Success Status</span> - Positive feedback</p>
                <p><span class="badge badge-warning">Warning Status</span> - Important notices</p>
                <p><span class="badge badge-danger">Danger Status</span> - Critical alerts</p>
            </div>
        </div>

        <div class="box-secondary">
            <h2>🌟 Get Started Today</h2>
            <p>Ready to transform your online presence? Our expert team is here to help you create a stunning website that reflects your brand and achieves your business goals. Contact us today to get started!</p>
            <button>Get In Touch</button>
            <button class="button-secondary">View Portfolio</button>
        </div>

        <h3>🎨 Our Color Palette</h3>
        <p>Our carefully selected color scheme combines professional blues with modern accents, creating a clean and trustworthy appearance that works for any industry.</p>
    </div>

    <script>
        document.getElementById('healthScoreForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            // Get form values
            const weight = parseFloat(document.getElementById('weight').value);
            const height = parseFloat(document.getElementById('height').value);
            const dob = new Date(document.getElementById('dob').value);
            
            // Validate inputs
            if (weight <= 0 || height <= 0) {
                alert('Please enter valid weight and height values');
                return;
            }
            
            // Calculate BMI using formula: BMI = weight / (height)^2
            const bmi = weight / (height * height);
            
            // Calculate age
            const today = new Date();
            let age = today.getFullYear() - dob.getFullYear();
            const monthDiff = today.getMonth() - dob.getMonth();
            if (monthDiff < 0 || (monthDiff === 0 && today.getDate() < dob.getDate())) {
                age--;
            }
            
            // Determine BMI category
            let category = '';
            let categoryColor = '';
            let indicatorColor = '';
            
            if (bmi < 18.5) {
                category = 'Underweight';
                categoryColor = '#2196F3';
                indicatorColor = '#2196F3';
            } else if (bmi >= 18.5 && bmi < 25) {
                category = 'Normal Weight';
                categoryColor = '#4CAF50';
                indicatorColor = '#4CAF50';
            } else if (bmi >= 25 && bmi < 30) {
                category = 'Overweight';
                categoryColor = '#FF9800';
                indicatorColor = '#FF9800';
            } else {
                category = 'Obesity';
                categoryColor = '#F44336';
                indicatorColor = '#F44336';
            }
            
            // Display results
            document.getElementById('age').textContent = age;
            document.getElementById('bmiValue').textContent = bmi.toFixed(2);
            document.getElementById('bmiValue').style.color = categoryColor;
            document.getElementById('bmiCategory').textContent = category;
            document.getElementById('bmiCategory').style.color = categoryColor;
            
            // Set indicator circle
            const indicator = document.getElementById('bmiIndicator');
            indicator.textContent = bmi.toFixed(1);
            indicator.style.backgroundColor = indicatorColor;
            
            // Show results section
            document.getElementById('result').classList.add('show');
        });
    </script>

</body>
</html>
