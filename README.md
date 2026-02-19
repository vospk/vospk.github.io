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

    </style>
</head>
<body>

    <div class="container">
        <h1> Welcome to Vospk</h1>

        <div class="box">
            <h2>About Us</h2>
            <p>At our core, we are dedicated to empowering individuals with smarter, data-driven health insights. Our disease prediction platform uses advanced algorithms and intelligent analysis to assess symptoms, lifestyle factors, and health indicators to provide personalized risk evaluations. Beyond prediction, our website offers tailored health recommendations, practical wellness advice, and an easy-to-understand health score that reflects your overall well-being. We believe that preventive care starts with awareness, and our mission is to make reliable health guidance accessible, simple, and actionable for everyone. By combining technology with health expertise, we aim to help you make informed decisions and take proactive steps toward a healthier future.</p>
            <button>Learn More</button>
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

</body>
</html>
