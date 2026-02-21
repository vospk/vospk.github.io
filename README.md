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

        /* Recommendation Styles */
        .recommendation-box {
            margin-top: 30px;
            padding: 20px;
            background-color: white;
            border-radius: 8px;
            border-left: 5px solid #0077B6;
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.1);
            display: none;
        }

        .recommendation-box.show {
            display: block;
        }

        .recommendation-box h4 {
            color: #0077B6;
            margin-top: 0;
            font-size: 18px;
        }

        .recommendation-text {
            color: #023047;
            font-size: 16px;
            line-height: 1.6;
            margin: 10px 0;
        }

        .recommendation-list {
            color: #023047;
            font-size: 15px;
            margin: 15px 0;
        }

        .recommendation-list li {
            margin: 8px 0;
            margin-left: 20px;
        }

        .scale-container {
            margin: 20px 0;
            padding: 15px;
            background-color: #f9f9f9;
            border-radius: 8px;
        }

        .scale-item {
            display: flex;
            align-items: center;
            margin: 10px 0;
        }

        .scale-dot {
            width: 15px;
            height: 15px;
            border-radius: 50%;
            margin-right: 10px;
        }

        .scale-label {
            color: #023047;
            font-weight: bold;
            font-size: 14px;
        }

        /* Obesity Section Styles */
        .obesity-section {
            background-color: #FFEBEE;
            padding: 20px;
            border-radius: 8px;
            border-left: 5px solid #D32F2F;
            margin-top: 20px;
            display: none;
        }

        .obesity-section.show {
            display: block;
        }

        .obesity-section h5 {
            color: #B71C1C;
            font-size: 18px;
            margin-top: 0;
            margin-bottom: 15px;
        }

        .subsection {
            margin-bottom: 20px;
        }

        .subsection-title {
            color: #C62828;
            font-weight: bold;
            font-size: 16px;
            margin-bottom: 10px;
            display: flex;
            align-items: center;
        }

        .section-emoji {
            margin-right: 10px;
            font-size: 20px;
        }

        .subsection-content {
            background-color: white;
            padding: 12px;
            border-radius: 5px;
            color: #023047;
            line-height: 1.6;
        }

        .tips-list {
            list-style: none;
            padding-left: 0;
        }

        .tips-list li {
            background-color: white;
            padding: 10px;
            margin: 8px 0;
            border-radius: 5px;
            border-left: 3px solid #D32F2F;
            color: #023047;
        }

        .warning-box {
            background-color: #FFF3E0;
            padding: 15px;
            border-radius: 5px;
            border-left: 5px solid #F57C00;
            margin-top: 15px;
        }

        .warning-box h6 {
            color: #E65100;
            margin-top: 0;
            font-size: 15px;
        }

        .warning-box p {
            color: #023047;
            margin: 8px 0;
            font-size: 14px;
        }

        .critical-warning {
            background-color: #FFCDD2;
            padding: 15px;
            border-radius: 5px;
            border-left: 5px solid #C62828;
            margin-top: 15px;
        }

        .critical-warning h6 {
            color: #B71C1C;
            margin-top: 0;
            font-size: 15px;
            font-weight: bold;
        }

        .critical-warning p {
            color: #023047;
            margin: 8px 0;
            font-size: 14px;
        }

        .critical-warning ul {
            margin: 10px 0;
            padding-left: 20px;
        }

        .critical-warning li {
            color: #023047;
            margin: 6px 0;
        }

        .dont-box {
            background-color: #FCE4EC;
            padding: 15px;
            border-radius: 5px;
            border-left: 5px solid #C2185B;
            margin-top: 15px;
        }

        .dont-box h6 {
            color: #880E4F;
            margin-top: 0;
            font-size: 15px;
        }

        .dont-list {
            list-style: none;
            padding-left: 0;
        }

        .dont-list li {
            color: #023047;
            margin: 8px 0;
            padding-left: 20px;
            position: relative;
        }

        .dont-list li:before {
            content: "✕";
            position: absolute;
            left: 0;
            color: #C2185B;
            font-weight: bold;
        }

        .goal-box {
            background-color: #E0F2F1;
            padding: 15px;
            border-radius: 5px;
            border-left: 5px solid #00897B;
            margin-top: 15px;
        }

        .goal-box h6 {
            color: #004D40;
            margin-top: 0;
            font-size: 15px;
        }

        .goal-box p {
            color: #023047;
            margin: 8px 0;
            font-size: 14px;
        }

        .goal-box ul {
            margin: 10px 0;
            padding-left: 20px;
        }

        .goal-box li {
            color: #023047;
            margin: 6px 0;
        }

        .reminder-box {
            background-color: #FCE4EC;
            padding: 15px;
            border-radius: 5px;
            border-left: 5px solid #E91E63;
            margin-top: 15px;
        }

        .reminder-box h6 {
            color: #880E4F;
            margin-top: 0;
            font-size: 15px;
        }

        .reminder-box p {
            color: #023047;
            margin: 8px 0;
            font-size: 14px;
        }

        .reminder-box ul {
            margin: 10px 0;
            padding-left: 20px;
        }

        .reminder-box li {
            color: #023047;
            margin: 6px 0;
        }

        .success-checkmark {
            color: #2ECC71;
            font-weight: bold;
            margin-right: 8px;
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
            <h2>Health Score</h2>
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

                <!-- Recommendation Section -->
                <div id="recommendationBox" class="recommendation-box">
                    <h4>📋 Health Recommendations</h4>
                    <div class="recommendation-text" id="recommendationText"></div>
                    
                    <div class="scale-container">
                        <strong style="color: #0077B6;">Health Status Scale:</strong>
                        <div class="scale-item">
                            <div class="scale-dot" style="background-color: #2196F3;"></div>
                            <span class="scale-label">Underweight - Below 18.5</span>
                        </div>
                        <div class="scale-item">
                            <div class="scale-dot" style="background-color: #4CAF50;"></div>
                            <span class="scale-label">Normal Weight - 18.5 to 24.9</span>
                        </div>
                        <div class="scale-item">
                            <div class="scale-dot" style="background-color: #FF9800;"></div>
                            <span class="scale-label">Overweight - 25.0 to 29.9</span>
                        </div>
                        <div class="scale-item">
                            <div class="scale-dot" style="background-color: #F44336;"></div>
                            <span class="scale-label">Obesity - 30.0 and above</span>
                        </div>
                    </div>
                    
                    <ul class="recommendation-list" id="recommendationList"></ul>
                </div>

                <!-- Obesity Detailed Section -->
                <div id="obesityDetailSection" class="obesity-section">
                    <h5>⚠️ Obesity Health Management Guide</h5>

                    <!-- Confirm with Healthcare Professional -->
                    <div class="subsection">
                        <div class="subsection-title">
                            <span class="section-emoji">✅ 1.</span>
                            <span>Confirm With a Healthcare Professional</span>
                        </div>
                        <div class="subsection-content">
                            <p style="margin: 0;"><strong style="color: #C62828;">A doctor should assess BMI along with growth charts (for teens), waist size, blood pressure, and overall health.</strong></p>
                            <p style="margin: 8px 0;">BMI alone does not tell the full story.</p>
                        </div>
                    </div>

                    <!-- Focus on Health -->
                    <div class="subsection">
                        <div class="subsection-title">
                            <span class="section-emoji">✅ 2.</span>
                            <span>Focus on Health, Not Just Weight</span>
                        </div>
                        <div class="subsection-content">
                            <p style="margin: 0;"><strong style="color: #C62828;">The goal is to improve health habits — not to "diet hard" or lose weight fast.</strong></p>
                            <p style="margin: 8px 0;">Small, sustainable changes lead to lasting results.</p>
                        </div>
                    </div>

                    <!-- Improve Eating Habits -->
                    <div class="subsection">
                        <div class="subsection-title">
                            <span class="section-emoji">🥗 3.</span>
                            <span>Improve Eating Habits (Gradual Changes)</span>
                        </div>
                        <div class="subsection-content">
                            <strong style="color: #C62828;">Do This:</strong>
                            <ul class="tips-list">
                                <li>Eat 3 balanced meals daily (don't skip meals)</li>
                                <li>Fill half your plate with vegetables or fruit</li>
                                <li>Choose whole grains instead of refined carbs</li>
                                <li>Include protein (eggs, beans, fish, chicken, yogurt)</li>
                                <li>Drink mostly water</li>
                                <li>Reduce sugary drinks and processed snacks</li>
                            </ul>
                            <strong style="color: #C62828; margin-top: 10px; display: block;">🚫 Avoid:</strong>
                            <ul class="tips-list">
                                <li>Crash diets or cutting out entire food groups</li>
                                <li>Skipping meals</li>
                                <li>Extreme restriction</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Increase Physical Activity -->
                    <div class="subsection">
                        <div class="subsection-title">
                            <span class="section-emoji">🚶 4.</span>
                            <span>Increase Physical Activity Slowly</span>
                        </div>
                        <div class="subsection-content">
                            <strong style="color: #C62828;">For teens:</strong>
                            <ul class="tips-list">
                                <li>Aim for about 60 minutes of movement daily</li>
                                <li>Start simple: walking, cycling, swimming, sports, dancing</li>
                                <li>Add light strength training 2–3 times per week</li>
                                <li>Start small if needed — even 10–15 minutes at first is okay</li>
                                <li>Pick activities you enjoy to stay motivated</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Sleep & Screen Time -->
                    <div class="subsection">
                        <div class="subsection-title">
                            <span class="section-emoji">😴 5.</span>
                            <span>Sleep & Screen Time</span>
                        </div>
                        <div class="subsection-content">
                            <ul class="tips-list">
                                <li>8–10 hours of sleep each night</li>
                                <li>Reduce late-night screen time</li>
                                <li>Poor sleep affects hunger hormones</li>
                                <li>Set a consistent sleep schedule</li>
                            </ul>
                        </div>
                    </div>

                    <!-- Critical Warning -->
                    <div class="critical-warning">
                        <h6>⚠️ See a Doctor If There Is:</h6>
                        <ul style="margin: 10px 0; padding-left: 20px;">
                            <li>Shortness of breath</li>
                            <li>Joint pain</li>
                            <li>Extreme fatigue</li>
                            <li>Family history of diabetes or heart disease</li>
                        </ul>
                        <p><strong>Medical guidance is important for safe progress.</strong></p>
                    </div>

                    <!-- Healthy Goal -->
                    <div class="goal-box">
                        <h6>🎯 Healthy Goal</h6>
                        <p><strong>For teens, the goal is often:</strong></p>
                        <ul style="margin: 10px 0; padding-left: 20px;">
                            <li>Growing taller while weight stays stable</li>
                            <li>Or slow, gradual weight reduction (if doctor recommends)</li>
                        </ul>
                        <p><strong>Safe change is slow — usually no more than 0.25–0.5 kg (0.5–1 lb) per week.</strong></p>
                    </div>

                    <!-- Important Reminder -->
                    <div class="reminder-box">
                        <h6>💛 Important Reminder</h6>
                        <ul style="margin: 10px 0; padding-left: 20px;">
                            <li>Avoid weight-loss pills or extreme diets</li>
                            <li>Don't compare yourself to social media</li>
                            <li>Health improvements matter more than fast results</li>
                            <li>You are worthy regardless of your weight</li>
                            <li>Seek support from family, friends, or professionals</li>
                        </ul>
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
        const recommendations = {
            underweight: {
                summary: "You are <strong>Underweight</strong>. While you may not have excess weight, it's important to ensure you're getting adequate nutrition and maintaining overall health.",
                tips: [
                    "Eat nutrient-dense foods with healthy calories (nuts, avocados, olive oil, whole grains)",
                    "Increase protein intake to support muscle development (lean meats, fish, legumes, dairy)",
                    "Eat 5-6 smaller meals throughout the day instead of 3 large meals",
                    "Include healthy fats from fish, seeds, and nut butters",
                    "Consult a healthcare provider to rule out any underlying health issues",
                    "Consider strength training to build muscle mass",
                    "Stay hydrated and get adequate sleep for overall wellness"
                ],
                showDetailSection: null
            },
            normal: {
                summary: "You have a <strong>Normal Weight</strong> range. Congratulations! You're in a healthy weight category. Focus on maintaining this through balanced nutrition and regular exercise.",
                tips: [
                    "Continue eating a balanced diet rich in fruits, vegetables, whole grains, and lean proteins",
                    "Aim for 150 minutes of moderate aerobic activity per week",
                    "Maintain consistent exercise habits (cardio, strength training, flexibility work)",
                    "Stay hydrated by drinking adequate water daily",
                    "Get 7-9 hours of quality sleep each night",
                    "Monitor your weight regularly to catch any changes early",
                    "Manage stress through meditation, yoga, or other relaxation techniques",
                    "Limit processed foods, sugar, and excessive salt intake"
                ],
                showDetailSection: null
            },
            overweight: {
                summary: "You are <strong>Overweight</strong>. While not in the obesity range, reducing weight gradually can improve your overall health and reduce disease risk.",
                tips: [
                    "Consult a healthcare provider or nutritionist for personalized advice",
                    "Create a modest calorie deficit (500 calories/day for gradual weight loss)",
                    "Increase daily physical activity gradually (start with 30 minutes most days)",
                    "Reduce portion sizes and eat slowly to improve satiety",
                    "Eliminate sugary drinks and limit alcohol consumption",
                    "Increase fiber intake through vegetables, fruits, and whole grains",
                    "Practice mindful eating - avoid eating while distracted",
                    "Set realistic weight loss goals (0.5-1 kg per week is healthy)",
                    "Track food intake to become aware of eating patterns",
                    "Find physical activities you enjoy to maintain consistency"
                ],
                showDetailSection: null
            },
            obesity: {
                summary: "You are in the <strong>Obesity</strong> category. This requires immediate lifestyle changes to reduce health risks including heart disease, diabetes, and other conditions.",
                tips: [
                    "Seek professional medical guidance from a doctor or health specialist immediately",
                    "Consider working with a registered dietitian for a personalized nutrition plan",
                    "Start with low-impact exercise like walking, swimming, or cycling (15-20 minutes daily)",
                    "Gradually increase exercise duration and intensity as fitness improves",
                    "Focus on whole foods: lean proteins, vegetables, fruits, whole grains",
                    "Reduce calorie intake progressively and avoid crash diets",
                    "Eliminate sugary beverages, fried foods, and processed snacks",
                    "Practice portion control using smaller plates",
                    "Address emotional eating and develop healthy coping mechanisms",
                    "Join a support group or consider behavioral therapy",
                    "Monitor weight weekly but focus on long-term sustainable changes",
                    "Sleep adequately and manage stress - both affect weight management",
                    "Set small achievable goals and celebrate progress",
                    "Consider medical interventions if recommended by your doctor"
                ],
                showDetailSection: 'obesity'
            }
        };

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
            let categoryKey = '';
            
            if (bmi < 18.5) {
                category = 'Underweight';
                categoryColor = '#2196F3';
                indicatorColor = '#2196F3';
                categoryKey = 'underweight';
            } else if (bmi >= 18.5 && bmi < 25) {
                category = 'Normal Weight';
                categoryColor = '#4CAF50';
                indicatorColor = '#4CAF50';
                categoryKey = 'normal';
            } else if (bmi >= 25 && bmi < 30) {
                category = 'Overweight';
                categoryColor = '#FF9800';
                indicatorColor = '#FF9800';
                categoryKey = 'overweight';
            } else {
                category = 'Obesity';
                categoryColor = '#F44336';
                indicatorColor = '#F44336';
                categoryKey = 'obesity';
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
            
            // Display recommendations
            const recData = recommendations[categoryKey];
            document.getElementById('recommendationText').innerHTML = recData.summary;
            
            const recList = document.getElementById('recommendationList');
            recList.innerHTML = '';
            recData.tips.forEach(tip => {
                const li = document.createElement('li');
                li.textContent = tip;
                recList.appendChild(li);
            });
            
            // Hide obesity detail section
            document.getElementById('obesityDetailSection').classList.remove('show');
            
            // Show appropriate detail section
            if (recData.showDetailSection === 'obesity') {
                document.getElementById('obesityDetailSection').classList.add('show');
            }
            
            // Show results and recommendations
            document.getElementById('result').classList.add('show');
            document.getElementById('recommendationBox').classList.add('show');
            
            // Scroll to results
            setTimeout(() => {
                document.getElementById('result').scrollIntoView({ behavior: 'smooth' });
            }, 100);
        });
    </script>

</body>
</html>
