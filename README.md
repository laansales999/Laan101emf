<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exquisite Madiwa Flavors | Premium Culinary Experiences</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;500;600;700&display=swap" rel="stylesheet">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }
        
        :root {
            --primary-blue: #0ea5e9;
            --dark-blue: #0a192f;
            --gold: #f59e0b;
            --light-bg: rgba(255, 255, 255, 0.05);
            --light-text: #f8f8f8;
            --dark-text: #1e293b;
            --header-blue: #0c4a6e;
        }
        
        body {
            background: linear-gradient(135deg, var(--dark-blue) 0%, #1e3a8a 100%);
            color: var(--light-text);
            line-height: 1.6;
            min-height: 100vh;
            display: flex;
            flex-direction: column;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
            flex: 1;
        }
        
        /* Header Styles */
        header {
            background: var(--header-blue);
            padding: 15px 0;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.15);
            position: sticky;
            top: 0;
            z-index: 1000;
        }
        
        .header-content {
            max-width: 1200px;
            margin: 0 auto;
            display: flex;
            align-items: center;
            justify-content: center;
            padding: 0 20px;
        }
        
        .logo-container {
            display: flex;
            align-items: center;
            gap: 15px;
        }
        
        .logo-img {
            height: 60px;
            width: auto;
        }
        
        .logo-text {
            font-size: 1.8rem;
            font-weight: 800;
            background: linear-gradient(135deg, var(--primary-blue), var(--gold));
            -webkit-background-clip: text;
            -webkit-text-fill-color: transparent;
        }
        
        /* Main Content Styles */
        .tagline {
            font-style: italic;
            color: var(--gold);
            margin-bottom: 20px;
            text-align: center;
        }
        
        .location-prompt {
            background: rgba(14, 165, 233, 0.15);
            padding: 20px;
            border-radius: 10px;
            text-align: center;
            margin-bottom: 30px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .location-prompt h2 {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
        }
        
        .btn {
            background: var(--gold);
            color: white;
            border: none;
            padding: 12px 25px;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            transition: all 0.3s ease;
            display: inline-block;
            margin-top: 15px;
        }
        
        .btn:hover {
            background: #d97706;
            transform: translateY(-2px);
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.2);
        }
        
        .event-section {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            margin-bottom: 40px;
            align-items: center;
        }
        
        .event-image {
            flex: 1;
            min-width: 300px;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .event-image img {
            width: 100%;
            height: auto;
            display: block;
        }
        
        .event-description {
            flex: 2;
            min-width: 300px;
            background: var(--light-bg);
            padding: 25px;
            border-radius: 10px;
            backdrop-filter: blur(10px);
        }
        
        .event-description h2 {
            color: var(--primary-blue);
            margin-bottom: 15px;
            font-size: 28px;
        }
        
        .event-description p {
            margin-bottom: 15px;
            font-size: 16px;
            line-height: 1.8;
        }
        
        .exclusive-tag {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            color: white;
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 14px;
            font-weight: 600;
            display: inline-block;
            margin-bottom: 15px;
        }
        
        .emf-poster {
            text-align: center;
            margin: 40px 0;
        }
        
        .emf-poster img {
            max-width: 100%;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.3);
        }
        
        .special-offer {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            padding: 15px;
            border-radius: 10px;
            text-align: center;
            margin: 20px 0;
            animation: pulse 2s infinite;
        }
        
        .menu-section {
            margin: 40px 0;
        }
        
        .menu-category {
            margin-bottom: 40px;
        }
        
        .menu-category h3 {
            color: var(--primary-blue);
            border-bottom: 2px solid var(--primary-blue);
            padding-bottom: 10px;
            margin-bottom: 20px;
            font-size: 24px;
        }
        
        .menu-items {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 20px;
        }
        
        .menu-item {
            background: var(--light-bg);
            border-radius: 10px;
            padding: 20px;
            transition: all 0.3s ease;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .menu-item:hover {
            transform: translateY(-5px);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .item-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 10px;
        }
        
        .item-name {
            font-weight: 600;
            font-size: 18px;
            color: var(--light-text);
        }
        
        .item-price {
            color: var(--gold);
            font-weight: 700;
        }
        
        .item-desc {
            color: #cbd5e1;
            font-size: 14px;
            margin-bottom: 15px;
        }
        
        .size-options {
            display: flex;
            gap: 10px;
            margin-bottom: 15px;
            flex-wrap: wrap;
        }
        
        .size-btn {
            padding: 5px 10px;
            border-radius: 20px;
            border: 1px solid var(--primary-blue);
            background: transparent;
            color: var(--light-text);
            cursor: pointer;
            font-size: 12px;
            transition: all 0.3s ease;
        }
        
        .size-btn.active {
            background: var(--primary-blue);
            color: white;
        }
        
        .item-controls {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .quantity-controls {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .quantity-btn {
            background: var(--primary-blue);
            color: white;
            border: none;
            width: 30px;
            height: 30px;
            border-radius: 50%;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
        }
        
        .quantity {
            font-weight: 600;
            width: 30px;
            text-align: center;
        }
        
        .limited-edition {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            color: white;
            padding: 3px 10px;
            border-radius: 15px;
            font-size: 12px;
            font-weight: 600;
            display: inline-block;
            margin-top: 10px;
        }
        
        .item-image {
            width: 100%;
            height: 180px;
            border-radius: 8px;
            overflow: hidden;
            margin-bottom: 12px;
        }
        
        .item-image img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        
        /* Drink Sizes Section */
        .drink-sizes {
            text-align: center;
            margin: 40px 0;
            padding: 20px;
            background: var(--light-bg);
            border-radius: 10px;
            backdrop-filter: blur(10px);
        }
        
        .drink-sizes h3 {
            color: var(--primary-blue);
            margin-bottom: 20px;
        }
        
        .size-comparison {
            max-width: 600px;
            margin: 0 auto;
            border-radius: 10px;
            overflow: hidden;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        /* Payment Method */
        .payment-method {
            background: var(--light-bg);
            padding: 20px;
            border-radius: 10px;
            margin: 20px 0;
            text-align: center;
            backdrop-filter: blur(10px);
        }
        
        .payment-method h3 {
            color: var(--primary-blue);
            margin-bottom: 15px;
        }
        
        .mpesa-details {
            background: rgba(0, 128, 0, 0.2);
            padding: 15px;
            border-radius: 8px;
            margin-top: 15px;
        }
        
        /* Floating Cart */
        .floating-cart {
            position: fixed;
            bottom: 20px;
            right: 20px;
            background: var(--light-bg);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 10px;
            padding: 15px;
            width: 320px;
            box-shadow: 0 5px 25px rgba(0, 0, 0, 0.3);
            z-index: 1000;
            max-height: 400px;
            overflow-y: auto;
            display: none;
        }
        
        .cart-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
            padding-bottom: 10px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .cart-items {
            max-height: 200px;
            overflow-y: auto;
            margin-bottom: 15px;
        }
        
        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 8px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
            font-size: 14px;
        }
        
        .cart-item-info {
            flex: 2;
        }
        
        .cart-item-controls {
            display: flex;
            align-items: center;
            gap: 8px;
        }
        
        .remove-btn {
            color: #ef4444;
            background: none;
            border: none;
            cursor: pointer;
            font-size: 14px;
        }
        
        .cart-total {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-weight: 700;
            font-size: 18px;
            padding-top: 10px;
            border-top: 2px solid rgba(255, 255, 255, 0.1);
        }
        
        .checkout-btn {
            width: 100%;
            padding: 12px;
            background: linear-gradient(135deg, #10b981, #059669);
            color: white;
            border: none;
            border-radius: 50px;
            font-weight: 600;
            font-size: 16px;
            cursor: pointer;
            transition: all 0.3s ease;
            margin-top: 15px;
        }
        
        .checkout-form {
            background: var(--light-bg);
            border-radius: 10px;
            padding: 25px;
            margin-top: 40px;
            display: none;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .form-group {
            margin-bottom: 20px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
        }
        
        .form-group input, .form-group textarea {
            width: 100%;
            padding: 12px 15px;
            border-radius: 8px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            background: rgba(255, 255, 255, 0.1);
            color: white;
        }
        
        .form-group input:focus, .form-group textarea:focus {
            outline: none;
            border-color: var(--primary-blue);
        }
        
        .whatsapp-chat {
            position: fixed;
            bottom: 90px;
            right: 20px;
            background: #25D366;
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 28px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
            z-index: 1000;
            transition: all 0.3s ease;
        }
        
        .whatsapp-chat:hover {
            transform: scale(1.1);
        }
        
        .cart-toggle {
            position: fixed;
            bottom: 20px;
            left: 20px;
            background: var(--gold);
            color: white;
            width: 60px;
            height: 60px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 24px;
            box-shadow: 0 4px 15px rgba(0, 0, 0, 0.3);
            z-index: 1000;
            transition: all 0.3s ease;
            cursor: pointer;
        }
        
        .cart-badge {
            position: absolute;
            top: -5px;
            right: -5px;
            background: #ef4444;
            color: white;
            width: 24px;
            height: 24px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 12px;
            font-weight: 600;
        }
        
        /* Footer Styles */
        footer {
            background: var(--header-blue);
            padding: 40px 0 20px;
            margin-top: 60px;
        }
        
        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
            gap: 30px;
        }
        
        .footer-about h3, .footer-contact h3 {
            color: var(--gold);
            margin-bottom: 15px;
            font-size: 1.2rem;
        }
        
        .footer-about p {
            line-height: 1.6;
            margin-bottom: 15px;
        }
        
        .footer-contact p {
            display: flex;
            align-items: center;
            gap: 10px;
            margin-bottom: 10px;
        }
        
        .footer-bottom {
            text-align: center;
            padding-top: 30px;
            margin-top: 30px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.02); }
            100% { transform: scale(1); }
        }
        
        @media (max-width: 768px) {
            .event-section {
                flex-direction: column;
            }
            
            .menu-items {
                grid-template-columns: 1fr;
            }
            
            .floating-cart {
                width: 90%;
                left: 5%;
                right: 5%;
                bottom: 80px;
            }
            
            .footer-content {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="header-content">
            <div class="logo-container">
                <img src="https://i.postimg.cc/3wZc6y70/laansale-logo.png" alt="Laansale Logo" class="logo-img">
                <div class="logo-text">Exquisite Madiwa Flavors</div>
            </div>
        </div>
    </header>

    <div class="container">
        <div class="tagline">Premium Culinary Experiences</div>

        <!-- Location Prompt Section -->
        <section class="location-prompt">
            <h2><i class="fas fa-location-dot"></i> Enable Your Location</h2>
            <p>To serve you better and provide accurate delivery, please enable location services</p>
            <button class="btn" id="enableLocation">Enable Location</button>
            <p id="locationStatus" style="margin-top: 15px;"></p>
        </section>

        <!-- Event Section -->
        <section class="event-section">
            <div class="event-image">
                <img src="https://i.postimg.cc/8zHQLv3L/event-poster.jpg" alt="Bustani Gardens Event">
            </div>
            <div class="event-description">
                <span class="exclusive-tag">EXCLUSIVE EVENT</span>
                <h2>Bustani Gardens Masterclass Experience</h2>
                <p>Join us for an exclusive culinary experience at Bustani Gardens, Red Hill. This is not just an event—it's a transformation for the top 0.00001% who understand that marketing excellence is the key to domination in any field.</p>
                <p>Laansale101 and Exquisite Madiwa Flavors present a fusion of elite taste and marketing mastery. Learn how to capture attention, create desire, and command loyalty through sensory experience.</p>
                <p>This is where the extraordinary is ordinary, and the exceptional is expected.</p>
                <button class="btn">Reserve Your Spot</button>
            </div>
        </section>

        <!-- EMF Poster Section -->
        <section class="emf-poster">
            <img src="https://i.postimg.cc/8zHQLv3L/event-poster.jpg" alt="EMF Feel Me More">
        </section>

        <!-- Drink Sizes Section -->
        <section class="drink-sizes">
            <h3>Our Drink Sizes</h3>
            <div class="size-comparison">
                <img src="https://i.postimg.cc/8zHQLv3L/event-poster.jpg" alt="Drink Size Comparison">
            </div>
            <p style="margin-top: 15px;">Now available in Small, Medium, and Large sizes</p>
        </section>

        <!-- Special Offer Banner -->
        <div class="special-offer">
            <h3>⏰ Limited Time Offer! 🚀</h3>
            <p>Order in the first 20 minutes of any hour and get 10% OFF your entire order!</p>
            <p id="countdown" style="font-weight: bold; margin-top: 10px;"></p>
        </div>

        <!-- Payment Method -->
        <div class="payment-method">
            <h3>Payment Method</h3>
            <p>We accept Lipa na M-Pesa</p>
            <div class="mpesa-details">
                <p><strong>PayBill:</strong> 542542</p>
                <p><strong>Account Number:</strong> 786867</p>
            </div>
        </div>

        <!-- Menu Section -->
        <section class="menu-section">
            <div class="menu-category">
                <h3>FRISS & 'KAK!</h3>
                <div class="menu-items">
                    <div class="menu-item">
                        <div class="item-image">
                            <img src="https://i.postimg.cc/3wZc6y70/laansale-logo.png" alt="Classic Crunch">
                        </div>
                        <div class="item-header">
                            <span class="item-name">Classic Crunch</span>
                            <span class="item-price">450/-</span>
                        </div>
                        <p class="item-desc">FRIES + 10 PCS MISHIKAKI + CHEF'S SIGNATURE SAUCE</p>
                        <span class="limited-edition">Limited Edition</span>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="classic-crunch">-</button>
                                <span class="quantity" data-item="classic-crunch">0</span>
                                <button class="quantity-btn plus" data-item="classic-crunch">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="classic-crunch" data-price="450">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-image">
                            <img src="https://i.postimg.cc/3wZc6y70/laansale-logo.png" alt="Grand Sultan">
                        </div>
                        <div class="item-header">
                            <span class="item-name">Grand Sultan</span>
                            <span class="item-price">550/-</span>
                        </div>
                        <p class="item-desc">MEGA LOADED FRIES WITH 15 PCS MSHIKAKI + SPECIAL SAUCE</p>
                        <p class="item-desc">EXTRA MSHIKAKI @100/- PER SKEWER</p>
                        <span class="limited-edition">Limited Edition</span>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="grand-sultan">-</button>
                                <span class="quantity" data-item="grand-sultan">0</span>
                                <button class="quantity-btn plus" data-item="grand-sultan">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="grand-sultan" data-price="550">Add to Cart</button>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="menu-category">
                <h3>FRESH JUICE</h3>
                <div class="menu-items">
                    <div class="menu-item">
                        <div class="item-image">
                            <img src="https://i.postimg.cc/3wZc6y70/laansale-logo.png" alt="Tangy Passion">
                        </div>
                        <div class="item-header">
                            <span class="item-name">Tangy Passion</span>
                            <span class="item-price" id="price-tangy-passion">250/-</span>
                        </div>
                        <p class="item-desc">Bold Passion, Pure Tropical Energy</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="tangy-passion" data-size="small" data-price="250">Small: 250/-</button>
                            <button class="size-btn" data-item="tangy-passion" data-size="medium" data-price="350">Medium: 350/-</button>
                            <button class="size-btn" data-item="tangy-passion" data-size="large" data-price="450">Large: 450/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="tangy-passion">-</button>
                                <span class="quantity" data-item="tangy-passion">0</span>
                                <button class="quantity-btn plus" data-item="tangy-passion">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="tangy-passion" data-price="250">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-image">
                            <img src="https://i.postimg.cc/3wZc6y70/laansale-logo.png" alt="Mango Rush">
                        </div>
                        <div class="item-header">
                            <span class="item-name">Mango Rush</span>
                            <span class="item-price" id="price-mango-rush">250/-</span>
                        </div>
                        <p class="item-desc">Thick, Juicy, Naturally Sweet</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="mango-rush" data-size="small" data-price="250">Small: 250/-</button>
                            <button class="size-btn" data-item="mango-rush" data-size="medium" data-price="350">Medium: 350/-</button>
                            <button class="size-btn" data-item="mango-rush" data-size="large" data-price="450">Large: 450/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="mango-rush">-</button>
                                <span class="quantity" data-item="mango-rush">0</span>
                                <button class="quantity-btn plus" data-item="mango-rush">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="mango-rush" data-price="250">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-image">
                            <img src="https://i.postimg.cc/3wZc6y70/laansale-logo.png" alt="Le' Pineapple De' Mint">
                        </div>
                        <div class="item-header">
                            <span class="item-name">Le' Pineapple De' Mint</span>
                            <span class="item-price" id="price-pineapple-mint">250/-</span>
                        </div>
                        <p class="item-desc">Altuty Breeze, Pineapple Squeeze</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="pineapple-mint" data-size="small" data-price="250">Small: 250/-</button>
                            <button class="size-btn" data-item="pineapple-mint" data-size="medium" data-price="350">Medium: 350/-</button>
                            <button class="size-btn" data-item="pineapple-mint" data-size="large" data-price="450">Large: 450/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="pineapple-mint">-</button>
                                <span class="quantity" data-item="pineapple-mint">0</span>
                                <button class="quantity-btn plus" data-item="pineapple-mint">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="pineapple-mint" data-price="250">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-image">
                            <img src="https://i.postimg.cc/3wZc6y70/laansale-logo.png" alt="Tropical Mix">
                        </div>
                        <div class="item-header">
                            <span class="item-name">Tropical Mix</span>
                            <span class="item-price" id="price-tropical-mix">250/-</span>
                        </div>
                        <p class="item-desc">All-in-one island infusion</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="tropical-mix" data-size="small" data-price="250">Small: 250/-</button>
                            <button class="size-btn" data-item="tropical-mix" data-size="medium" data-price="350">Medium: 350/-</button>
                            <button class="size-btn" data-item="tropical-mix" data-size="large" data-price="450">Large: 450/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="tropical-mix">-</button>
                                <span class="quantity" data-item="tropical-mix">0</span>
                                <button class="quantity-btn plus" data-item="tropical-mix">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="tropical-mix" data-price="250">Add to Cart</button>
                        </div>
                    </div>
                </div>
            </div>
            
            <div class="menu-category">
                <h3>MAGIC MOJITOS</h3>
                <div class="menu-items">
                    <div class="menu-item">
                        <div class="item-image">
                            <img src="https://i.postimg.cc/3wZc6y70/laansale-logo.png" alt="Blue Lagoon">
                        </div>
                        <div class="item-header">
                            <span class="item-name">Blue Lagoon</span>
                            <span class="item-price" id="price-blue-lagoon">300/-</span>
                        </div>
                        <p class="item-desc">Tropical Citrus Wave, Blue Ocean</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="blue-lagoon" data-size="small" data-price="300">Small: 300/-</button>
                            <button class="size-btn" data-item="blue-lagoon" data-size="medium" data-price="400">Medium: 400/-</button>
                            <button class="size-btn" data-item="blue-lagoon" data-size="large" data-price="500">Large: 500/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="blue-lagoon">-</button>
                                <span class="quantity" data-item="blue-lagoon">0</span>
                                <button class="quantity-btn plus" data-item="blue-lagoon">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="blue-lagoon" data-price="300">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-image">
                            <img src="https://i.postimg.cc/3wZc6y70/laansale-logo.png" alt="Red Flash">
                        </div>
                        <div class="item-header">
                            <span class="item-name">Red Flash</span>
                            <span class="item-price" id="price-red-flash">300/-</span>
                        </div>
                        <p class="item-desc">Bold strawberry heat meets cool mint</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="red-flash" data-size="small" data-price="300">Small: 300/-</button>
                            <button class="size-btn" data-item="red-flash" data-size="medium" data-price="400">Medium: 400/-</button>
                            <button class="size-btn" data-item="red-flash" data-size="large" data-price="500">Large: 500/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="red-flash">-</button>
                                <span class="quantity" data-item="red-flash">0</span>
                                <button class="quantity-btn plus" data-item="red-flash">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="red-flash" data-price="300">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-image">
                            <img src="https://i.postimg.cc/3wZc6y70/laansale-logo.png" alt="Berry Breeze">
                        </div>
                        <div class="item-header">
                            <span class="item-name">Berry Breeze</span>
                            <span class="item-price" id="price-berry-breeze">300/-</span>
                        </div>
                        <p class="item-desc">Smooth berry chill, island style</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="berry-breeze" data-size="small" data-price="300">Small: 300/-</button>
                            <button class="size-btn" data-item="berry-breeze" data-size="medium" data-price="400">Medium: 400/-</button>
                            <button class="size-btn" data-item="berry-breeze" data-size="large" data-price="500">Large: 500/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="berry-breeze">-</button>
                                <span class="quantity" data-item="berry-breeze">0</span>
                                <button class="quantity-btn plus" data-item="berry-breeze">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="berry-breeze" data-price="300">Add to Cart</button>
                        </div>
                    </div>
                    
                    <div class="menu-item">
                        <div class="item-image">
                            <img src="https://i.postimg.cc/3wZc6y70/laansale-logo.png" alt="Ginger Gold">
                        </div>
                        <div class="item-header">
                            <span class="item-name">Ginger Gold</span>
                            <span class="item-price" id="price-ginger-gold">300/-</span>
                        </div>
                        <p class="item-desc">Golden spice with honeyed flow</p>
                        <div class="size-options">
                            <button class="size-btn active" data-item="ginger-gold" data-size="small" data-price="300">Small: 300/-</button>
                            <button class="size-btn" data-item="ginger-gold" data-size="medium" data-price="400">Medium: 400/-</button>
                            <button class="size-btn" data-item="ginger-gold" data-size="large" data-price="500">Large: 500/-</button>
                        </div>
                        <div class="item-controls">
                            <div class="quantity-controls">
                                <button class="quantity-btn minus" data-item="ginger-gold">-</button>
                                <span class="quantity" data-item="ginger-gold">0</span>
                                <button class="quantity-btn plus" data-item="ginger-gold">+</button>
                            </div>
                            <button class="btn add-to-cart" data-item="ginger-gold" data-price="300">Add to Cart</button>
                        </div>
                    </div>
                </div>
            </div>
        </section>

        <!-- Checkout Form -->
        <section class="checkout-form" id="checkout-form">
            <h3>Complete Your Order</h3>
            <div class="form-group">
                <label for="name">Full Name</label>
                <input type="text" id="name" required>
            </div>
            <div class="form-group">
                <label for="phone">Phone Number</label>
                <input type="tel" id="phone" required>
            </div>
            <div class="form-group">
                <label for="dressing">Dressing Description (Optional)</label>
                <textarea id="dressing" rows="3"></textarea>
            </div>
            <div class="form-group">
                <label for="location">Delivery Location</label>
                <input type="text" id="delivery-location" readonly>
            </div>
            <button class="checkout-btn" id="place-order">Place Order via WhatsApp</button>
        </section>

        <!-- Floating Cart -->
        <div class="floating-cart" id="floating-cart">
            <div class="cart-header">
                <h3>Your Order</h3>
                <span id="cart-count">0 items</span>
            </div>
            <div class="cart-items" id="cart-items">
                <p style="text-align: center; padding: 20px;">Your cart is empty</p>
            </div>
            <div class="cart-total">
                <span>Total:</span>
                <span id="cart-total">0/-</span>
            </div>
            <button class="checkout-btn" id="checkout-btn">Proceed to Checkout</button>
        </div>

        <!-- Cart Toggle Button -->
        <div class="cart-toggle" id="cart-toggle">
            <i class="fas fa-shopping-cart"></i>
            <span class="cart-badge" id="cart-badge">0</span>
        </div>

        <!-- WhatsApp Chat -->
        <a href="https://wa.me/254115030726" class="whatsapp-chat" target="_blank">
            <i class="fab fa-whatsapp"></i>
        </a>
    </div>

    <footer>
        <div class="footer-content">
            <div class="footer-about">
                <h3>About Laansales101</h3>
                <p>Laansales101 was born from a deep understanding of the challenges that vendors and event-goers face. What if there was a way to merge convenience with luxury, to transform an ordinary event into an extraordinary experience? That vision led to the creation of Laansales101—a cutting-edge platform designed to make ordering seamless, effortless, and uniquely personal for every event-goer.</p>
            </div>
            <div class="footer-contact">
                <h3>Contact Us</h3>
                <p><i class="fas fa-envelope"></i> emflavorsales@gmail.com</p>
                <p><i class="fas fa-phone"></i> +254 115 030 726</p>
                <p><i class="fas fa-map-marker-alt"></i> Bustani Gardens, Red Hill</p>
            </div>
        </div>
        <div class="footer-bottom">
            <p>&copy; 2025 Laansales101. All Rights Reserved.</p>
        </div>
    </footer>

    <script>
        // Initialize cart
        let cart = [];
        let userLocation = null;
        
        // DOM Elements
        const enableLocationBtn = document.getElementById('enableLocation');
        const locationStatus = document.getElementById('locationStatus');
        const checkoutBtn = document.getElementById('checkout-btn');
        const checkoutForm = document.getElementById('checkout-form');
        const placeOrderBtn = document.getElementById('place-order');
        const deliveryLocation = document.getElementById('delivery-location');
        const countdownEl = document.getElementById('countdown');
        const floatingCart = document.getElementById('floating-cart');
        const cartToggle = document.getElementById('cart-toggle');
        const cartBadge = document.getElementById('cart-badge');
        
        // Enable location
        enableLocationBtn.addEventListener('click', () => {
            if (navigator.geolocation) {
                navigator.geolocation.getCurrentPosition(
                    position => {
                        userLocation = position;
                        const { latitude, longitude } = position.coords;
                        locationStatus.innerHTML = `Location enabled! Latitude: ${latitude.toFixed(6)}, Longitude: ${longitude.toFixed(6)}`;
                        locationStatus.style.color = '#10b981';
                        deliveryLocation.value = `${latitude.toFixed(6)}, ${longitude.toFixed(6)}`;
                        
                        // Try to get address from coordinates
                        getAddressFromCoords(latitude, longitude);
                    },
                    error => {
                        locationStatus.innerHTML = 'Unable to retrieve location. Please enable location permissions.';
                        locationStatus.style.color = '#ef4444';
                    }
                );
            } else {
                locationStatus.innerHTML = 'Geolocation is not supported by this browser.';
                locationStatus.style.color = '#ef4444';
            }
        });
        
        // Function to get address from coordinates using OpenStreetMap Nominatim
        function getAddressFromCoords(lat, lng) {
            fetch(`https://nominatim.openstreetmap.org/reverse?format=json&lat=${lat}&lon=${lng}`)
                .then(response => response.json())
                .then(data => {
                    if (data && data.display_name) {
                        deliveryLocation.value = data.display_name;
                    }
                })
                .catch(error => {
                    console.error('Error getting address from coordinates:', error);
                });
        }
        
        // Size selection for drinks
        document.querySelectorAll('.size-btn').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const size = button.getAttribute('data-size');
                const price = button.getAttribute('data-price');
                
                // Remove active class from all buttons in this group
                button.parentNode.querySelectorAll('.size-btn').forEach(btn => {
                    btn.classList.remove('active');
                });
                
                // Add active class to clicked button
                button.classList.add('active');
                
                // Update price display
                document.getElementById(`price-${item}`).textContent = `${price}/-`;
                
                // Update add to cart button data-price
                const addButton = button.closest('.menu-item').querySelector('.add-to-cart');
                addButton.setAttribute('data-price', price);
            });
        });
        
        // Quantity controls
        document.querySelectorAll('.quantity-btn').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const quantityEl = document.querySelector(`.quantity[data-item="${item}"]`);
                let quantity = parseInt(quantityEl.textContent);
                
                if (button.classList.contains('plus')) {
                    quantity++;
                } else if (button.classList.contains('minus') && quantity > 0) {
                    quantity--;
                }
                
                quantityEl.textContent = quantity;
            });
        });
        
        // Add to cart
        document.querySelectorAll('.add-to-cart').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const price = parseInt(button.getAttribute('data-price'));
                const quantity = parseInt(document.querySelector(`.quantity[data-item="${item}"]`).textContent);
                
                if (quantity === 0) return;
                
                // Get selected size for drinks
                let size = null;
                const sizeBtn = button.closest('.menu-item').querySelector('.size-btn.active');
                if (sizeBtn) {
                    size = sizeBtn.getAttribute('data-size');
                }
                
                // Check if item already in cart
                const existingItemIndex = cart.findIndex(cartItem => 
                    cartItem.name === item && cartItem.size === size
                );
                
                if (existingItemIndex !== -1) {
                    cart[existingItemIndex].quantity += quantity;
                } else {
                    cart.push({
                        name: item,
                        price: price,
                        quantity: quantity,
                        size: size
                    });
                }
                
                updateCart();
                
                // Reset quantity
                document.querySelector(`.quantity[data-item="${item}"]`).textContent = '0';
                
                // Show cart
                floatingCart.style.display = 'block';
            });
        });
        
        // Update cart
        function updateCart() {
            const cartItems = document.getElementById('cart-items');
            const cartCount = document.getElementById('cart-count');
            const cartTotal = document.getElementById('cart-total');
            
            // Clear cart items
            cartItems.innerHTML = '';
            
            if (cart.length === 0) {
                cartItems.innerHTML = '<p style="text-align: center; padding: 20px;">Your cart is empty</p>';
                cartCount.textContent = '0 items';
                cartTotal.textContent = '0/-';
                cartBadge.textContent = '0';
                return;
            }
            
            let total = 0;
            let itemCount = 0;
            
            cart.forEach((item, index) => {
                const itemTotal = item.price * item.quantity;
                total += itemTotal;
                itemCount += item.quantity;
                
                const cartItemEl = document.createElement('div');
                cartItemEl.className = 'cart-item';
                
                let sizeInfo = '';
                if (item.size) {
                    sizeInfo = ` (${item.size})`;
                }
                
                cartItemEl.innerHTML = `
                    <div class="cart-item-info">
                        <div>${formatItemName(item.name)}${sizeInfo}</div>
                        <div>${item.price}/- x ${item.quantity}</div>
                    </div>
                    <div class="cart-item-controls">
                        <span>${itemTotal}/-</span>
                        <button class="remove-btn" data-index="${index}">
                            <i class="fas fa-trash"></i>
                        </button>
                    </div>
                `;
                
                cartItems.appendChild(cartItemEl);
            });
            
            cartCount.textContent = `${itemCount} ${itemCount === 1 ? 'item' : 'items'}`;
            cartTotal.textContent = `${total}/-`;
            cartBadge.textContent = itemCount;
            
            // Add event listeners to remove buttons
            document.querySelectorAll('.remove-btn').forEach(button => {
                button.addEventListener('click', () => {
                    const index = parseInt(button.getAttribute('data-index'));
                    cart.splice(index, 1);
                    updateCart();
                });
            });
        }
        
        // Format item name for display
        function formatItemName(name) {
            return name.split('-')
                .map(word => word.charAt(0).toUpperCase() + word.slice(1))
                .join(' ');
        }
        
        // Toggle cart visibility
        cartToggle.addEventListener('click', () => {
            if (floatingCart.style.display === 'block') {
                floatingCart.style.display = 'none';
            } else {
                floatingCart.style.display = 'block';
            }
        });
        
        // Checkout button
        checkoutBtn.addEventListener('click', () => {
            if (cart.length === 0) {
                alert('Your cart is empty. Please add items before checkout.');
                return;
            }
            
            if (!userLocation) {
                alert('Please enable location services to proceed with checkout.');
                return;
            }
            
            checkoutForm.style.display = 'block';
            checkoutForm.scrollIntoView({ behavior: 'smooth' });
        });
        
        // Place order
        placeOrderBtn.addEventListener('click', () => {
            const name = document.getElementById('name').value;
            const phone = document.getElementById('phone').value;
            
            if (!name || !phone) {
                alert('Please fill in all required fields.');
                return;
            }
            
            // Create order summary
            let orderSummary = `*NEW ORDER FROM EXQUISITE MADIWA FLAVORS WEBSITE*\n\n`;
            orderSummary += `*Customer Name:* ${name}\n`;
            orderSummary += `*Phone:* ${phone}\n`;
            orderSummary += `*Location:* ${deliveryLocation.value}\n\n`;
            orderSummary += `*Order Details:*\n`;
            
            cart.forEach(item => {
                let sizeInfo = '';
                if (item.size) {
                    sizeInfo = ` (${item.size})`;
                }
                orderSummary += `- ${formatItemName(item.name)}${sizeInfo} x ${item.quantity} = ${item.price * item.quantity}/-\n`;
            });
            
            orderSummary += `\n*Total: ${cart.reduce((total, item) => total + (item.price * item.quantity), 0)}/-*\n\n`;
            
            const dressing = document.getElementById('dressing').value;
            if (dressing) {
                orderSummary += `*Dressing Instructions:* ${dressing}\n`;
            }
            
            orderSummary += `\n*Payment Method:* Lipa na M-Pesa\n`;
            orderSummary += `*PayBill:* 542542\n`;
            orderSummary += `*Account Number:* 786867\n`;
            
            // Encode for WhatsApp URL
            const encodedMessage = encodeURIComponent(orderSummary);
            const whatsappURL = `https://wa.me/254115030726?text=${encodedMessage}`;
            
            // Open WhatsApp
            window.open(whatsappURL, '_blank');
            
            // Reset cart and form
            cart = [];
            updateCart();
            checkoutForm.style.display = 'none';
            document.getElementById('name').value = '';
            document.getElementById('phone').value = '';
            document.getElementById('dressing').value = '';
            
            alert('Your order has been placed! You will be redirected to WhatsApp to confirm.');
        });
        
        // Countdown timer for special offer
        function updateCountdown() {
            const now = new Date();
            const minutes = now.getMinutes();
            const seconds = now.getSeconds();
            
            if (minutes < 20) {
                const timeLeft = 20 - minutes;
                const secsLeft = 60 - seconds;
                countdownEl.textContent = `Offer ends in: ${timeLeft} min ${secsLeft} sec`;
            } else {
                const nextHour = new Date(now);
                nextHour.setHours(nextHour.getHours() + 1);
                nextHour.setMinutes(0);
                nextHour.setSeconds(0);
                
                const diff = nextHour - now;
                const minsLeft = Math.floor(diff / 60000);
                const secsLeft = Math.floor((diff % 60000) / 1000);
                
                countdownEl.textContent = `Next offer in: ${minsLeft} min ${secsLeft} sec`;
            }
        }
        
        setInterval(updateCountdown, 1000);
        updateCountdown();
    </script>
</body>
</html>            --light-text: #f8f8f8;
            --dark-text: #1e293b;
            --transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }
        
        body {
            background: linear-gradient(135deg, var(--dark-blue) 0%, #1e3a8a 100%);
            color: var(--light-text);
            line-height: 1.6;
            padding-bottom: 80px;
            font-family: 'Poppins', sans-serif;
            overflow-x: hidden;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* NEW SIMPLIFIED HEADER STYLES */
        .main-header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 15px 0;
            background: var(--dark-blue);
            z-index: 10000;
            border-bottom: 2px solid var(--gold);
        }
        
        .logo-container {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .logo {
            width: 120px;
            height: auto;
            transition: var(--transition);
        }
        
        .logo:hover {
            transform: scale(1.05);
        }
        
        .tagline {
            font-style: italic;
            color: var(--gold);
            margin-top: 5px;
            font-size: 0.9rem;
            font-family: 'Playfair Display', serif;
        }
        
        /* Footer Styles */
        footer {
            background: var(--dark-blue);
            padding: 60px 0 30px;
            margin-top: 60px;
            border-top: 2px solid var(--gold);
            position: relative;
        }
        
        .footer-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 30px;
        }
        
        .footer-about {
            flex: 2;
            min-width: 300px;
        }
        
        .footer-about h3 {
            color: var(--gold);
            margin-bottom: 15px;
            font-size: 1.5rem;
            font-family: 'Playfair Display', serif;
        }
        
        .footer-about p {
            margin-bottom: 15px;
            line-height: 1.8;
            font-size: 0.95rem;
        }
        
        .footer-contact {
            flex: 1;
            min-width: 250px;
        }
        
        .footer-contact h3 {
            color: var(--gold);
            margin-bottom: 15px;
            font-size: 1.5rem;
            font-family: 'Playfair Display', serif;
        }
        
        .footer-contact p {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .footer-logo {
            text-align: center;
            margin-top: 30px;
        }
        
        .footer-logo img {
            width: 120px;
            opacity: 0.9;
        }
        
        .footer-bottom {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
        }
        
        /* Main Content */
        .main-content {
            padding-top: 100px;
        }
        
        .location-prompt {
            background: rgba(14, 165, 233, 0.15);
            padding: 25px;
            border-radius: 15px;
            text-align: center;
            margin-bottom: 40px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .location-prompt h2 {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            font-family: 'Playfair Display', serif;
        }
        
        .btn {
            background: var(--gold);
            color: white;
            border: none;
            padding: 14px 30px;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            transition: var(--transition);
            display: inline-block;
            margin-top: 15px;
            font-size: 1rem;
            letter-spacing: 0.5px;
            box-shadow: 0 4px 10px rgba(245, 158, 11, 0.3);
        }
        
        .btn:hover {
            background: #d97706;
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.2);
        }
        
        .event-section {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            margin-bottom: 50px;
            align-items: center;
        }
        
        .event-image {
            flex: 1;
            min-width: 300px;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            transition: var(--transition);
        }
        
        .event-image:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.4);
        }
        
        .event-image img {
            width: 100%;
            height: auto;
            display: block;
            transition: var(--transition);
        }
        
        .event-image:hover img {
            transform: scale(1.03);
        }
        
        .event-description {
            flex: 2;
            min-width: 300px;
            background: var(--light-bg);
            padding: 30px;
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .event-description h2 {
            color: var(--primary-blue);
            margin-bottom: 20px;
            font-size: 32px;
            font-family: 'Playfair Display', serif;
        }
        
        .event-description p {
            margin-bottom: 20px;
            font-size: 16px;
            line-height: 1.8;
        }
        
        .exclusive-tag {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            color: white;
            padding: 8px 20px;
            border-radius: 20px;
            font-size: 14px;
            font-weight: 600;
            display: inline-block;
            margin-bottom: 20px;
            letter-spacing: 0.5px;
        }
        
        .emf-poster {
            text-align: center;
            margin: 50px 0;
        }
        
        .emf-poster img {
            max-width: 100%;
            border-radius: 15px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            transition: var(--transition);
        }
        
        .emf-poster img:hover {
            transform: scale(1.02);
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.4);
        }
        
        .special-offer {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            padding: 20px;
            border-radius: 15px;
            text-align: center;
            margin: 30px 0;
            animation: pulse 2s infinite;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .special-offer h3 {
            font-size: 1.5rem;
            margin-bottom: 10px;
        }
        
        .menu-section {
            margin: 50px 0;
        }
        
        .menu-category {
            margin-bottom: 50px;
        }
        
        .menu-category h3 {
            color: var(--primary-blue);
            border-bottom: 2px solid var(--primary-blue);
            padding-bottom: 15px;
            margin-bottom: 30px;
            font-size: 28px;
            font-family: 'Playfair Display', serif;
        }
        
        .menu-items {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 25px;
        }
        
        .menu-item {
            background: var(--light-bg);
            border-radius: 15px;
            padding: 25px;
            transition: var(--transition);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        .menu-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(12, 77, 162, 0.1), rgba(245, 158, 11, 0.1));
            z-index: -1;
            opacity: 0;
            transition: var(--transition);
        }
        
        .menu-item:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.2);
        }
        
        .menu-item:hover::before {
            opacity: 1;
        }
        
        .item-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }
        
        .item-name {
            font-weight: 700;
            font-size: 20px;
            color: var(--light-text);
            font-family: 'Playfair Display', serif;
        }
        
        .item-price {
            color: var(--gold);
            font-weight: 800;
            font-size: 22px;
        }
        
        .item-desc {
            color: #cbd5e1;
            font-size: 15px;
            margin-bottom: 20px;
            line-height: 1.6;
        }
        
        .size-options {
            display: flex;
            gap: 10px;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }
        
        .size-btn {
            padding: 8px 15px;
            border-radius: 20px;
            border: 1px solid var(--primary-blue);
            background: transparent;
            color: var(--light-text);
            cursor: pointer;
            font-size: 13px;
            transition: var(--transition);
        }
        
        .size-btn.active {
            background: var(--primary-blue);
            color: white;
            box-shadow: 0 4px 10px rgba(12, 77, 162, 0.3);
        }
        
        .item-controls {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .quantity-controls {
            display: flex;
            align-items: center;
            gap: 12px;
        }
        
        .quantity-btn {
            background: var(--primary-blue);
            color: white;
            border: none;
            width: 35px;
            height: 35px;
            border-radius: 50%;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
            font-weight: bold;
        }
        
        .quantity-btn:hover {
            background: #0a3d80;
            transform: scale(1.1);
        }
        
        .quantity {
            font-weight: 700;
            width: 35px;
            text-align: center;
            font-size: 18px;
        }
        
        .limited-edition {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            color: white;
            padding: 5px 15px;
            border-radius: 15px;
            font-size: 13px;
            font-weight: 600;
            display: inline-block;
            margin-top: 15px;
            letter-spacing: 0.5px;
        }
        
        /* Drink Sizes Section */
        .drink-sizes {
            text-align: center;
            margin: 50px 0;
            padding: 30px;
            background: var(--light-bg);
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .drink-sizes h3 {
            color: var(--primary-blue);
            margin-bottom: 25px;
            font-size: 28px;
            font-family: 'Playfair Display', serif;
        }
        
        .drink-sizes img {
            max-width: 100%;
            border-radius: 15px;
            box-shadow: 0 8px极市 25px rgba(0, 0, 0, 0.3);
            transition: var(--transition);
        }
        
        .drink-sizes img:hover {
            transform: scale(1.02);
        }
        
        /* Floating Cart */
        .floating-cart {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: var(--light-bg);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 极市0.1);
            border-radius: 15px;
            padding: 20px;
            width: 350px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            z-index: 1000;
            max-height: 450px;
            overflow-y: auto;
            transition: var(--transition);
            transform: translateX(0);
        }
        
        .cart-hidden {
            transform: translateX(400px);
        }
        
        .cart-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 15px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .cart-header h3 {
            font-family: 'Playfair Display', serif;
            color: var(--gold);
        }
        
        .cart-items {
            max-height: 250px;
            overflow-y: auto;
            margin-bottom: 20px;
        }
        
        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 12px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
            font-size: 15px;
        }
        
        .cart-item-info {
            flex: 2;
        }
        
        .cart-item-controls {
            display:极市 flex;
            align-items: center;
            gap: 10px;
        }
        
        .remove-btn {
            color: #ef4444;
            background: none;
            border: none;
            cursor: pointer;
            font-size: 16px;
            transition: var(--transition);
        }
        
        .remove-btn:hover {
            transform: scale(1.2);
        }
        
        .cart-total {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-weight: 800;
            font-size: 20px;
            padding-top: 15px;
            border-top: 2px solid rgba(255, 255, 255, 0.1);
            color: var(--gold);
        }
        
        .checkout-btn {
            width: 100%;
            padding: 15px;
            background: linear-gradient(135deg, #10b981, #059669);
            color: white;
            border: none;
            border-radius: 50px;
            font-weight: 700;
            font-size: 16px;
            cursor: pointer;
            transition: var(--transition);
            margin-top: 20px;
            letter-spacing: 0.5px;
           极市 box-shadow: 0 5极市px 15px rgba(16, 185, 129, 0.3);
        }
        
        .checkout-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(16, 185, 129, 0.4);
        }
        
        .checkout-form {
            background: var(--light-bg);
            border-radius: 15极市px;
            padding: 30px;
            margin-top: 50px;
            display: none;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
        }
        
        .checkout-form h3 {
            color: var(--gold);
            margin-bottom: 25px;
            font-size: 28px;
            font-family: 'Playfair Display', serif;
            text-align: center;
        }
        
        .form-group {
            margin-bottom: 25px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 10px;
            font-weight: 600;
            font-size: 16px;
        }
        
        .form-group input, .form-group textarea, .form-group select {
            width: 100%;
            padding: 15px 20px;
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            background: rgba(255, 255, 255, 0.1);
            color: white;
            font-size: 16px;
            transition: var(--transition);
        }
        
        .form-group input:focus, .form-group textarea:focus, .form-group select:focus {
            outline: none;
            border-color: var(--primary-blue);
            box-shadow: 0 0 0 2px rgba(12, 77, 162, 0.3);
        }
        
        .payment-info {
            background: rgba(14, 165, 233, 0.1);
            padding: 20px;
            border-radius: 10px;
            margin: 25px 0;
            border-left: 4px solid var(--primary-blue);
        }
        
        .payment-info h4 {
            color: var(--gold);
            margin-bottom: 15px;
            font-size: 20px;
            font-family: 'Playfair Display', serif;
        }
        
        .payment-info p {
            margin-bottom: 10px;
        }
        
        .whatsapp-chat {
            position: fixed;
            bottom: 110px;
            right: 30px;
            background: #25D366;
            color: white;
            width: 65px;
            height: 65极市px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 30px;
            box-shadow: 0 6px 20px rgba(37, 211, 102, 0.4);
            z-index: 1000;
            transition: var(--transition);
        }
        
        .whatsapp-chat:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 25px rgba(37, 211, 102, 0.5);
        }
        
        .cart-toggle {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: var(--gold);
            color: white;
            width: 65px;
            height: 65px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 26px;
            box-shadow: 0 6px 20px rgba(245, 158, 11, 0.4);
            z-index: 1000;
            transition: var(--transition);
            cursor: pointer;
        }
        
        .cart-toggle:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 25px rgba(245, 158, 11, 0.5);
        }
        
        .cart-badge {
            position: absolute;
            top: -5px;
            right: -5px;
            background: #ef4444;
            color: white;
            width: 26px;
            height: 26px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 13px;
            font-weight: 700;
            box-shadow: 极市0 2px 8px rgba(239, 68, 68, 0.3);
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.02); }
            100% { transform: scale(1); }
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .fade-in {
            animation: fadeIn 1s ease forwards;
        }
        
        @media (max-width: 1024px) {
            .menu-items {
                grid-template-columns: repeat(auto-fill, minmax(280极市px, 1fr));
            }
        }
        
        @media (max-width: 768px) {
            .event-section {
                flex-direction: column;
            }
            
            .menu-items {
                grid-template-columns: 1fr;
            }
            
            .floating-c极市art {
                width: 90%;
                left: 5%;
                right: 5%;
                bottom: 100px;
            }
            
            .footer-content {
                flex-direction: column;
            }
            
            .cart-toggle {
                bottom: 20px;
                right: 20px;
            }
            
            .whatsapp-chat {
                bottom: 100px;
                right: 20px;
            }
            
            .main-header {
                padding: 8px 0;
                height: auto;
            }
            
            .logo {
                width: 100px;
            }
            
            .tagline {
                font-size: 0.8rem;
            }
            
            .main-content {
                padding-top: 90px;
            }
        }
        
        @media (max-width: 480px) {
            .container {
                padding: 15px;
            }
            
            .btn {
                padding: 12px 25px;
                font-size: 0.9rem;
            }
            
            .event-description {
                padding: 20px;
            }
            
            .menu-item {
                padding: 20px;
            }
            
            .item-name {
                font-size: 18px;
            }
            
            .item-price {
                font-size: 20px;
            }
            
            .main-header {
                padding: 10px 0;
            }
            
            .logo {
                width: 90px;
            }
            
            .tagline {
                display: none;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header with Logo -->
        <header class="main-header" id="main-header">
            <div class="logo-container">
                <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070816_Gallery.jpg" alt="Laansale Logo" class="logo">
                <div class="tagline">Premium Culinary Experiences</div>
            </div>
        </header>

        <div class="main-content">
            <!-- Location Prompt Section -->
            <section class="location-prompt fade-in">
                <h2><i class="fas fa-location-dot"></i> Enable Your Location</h2>
                <p>To serve you better and provide accurate delivery, please enable location services</p>
                <button class="btn" id="enableLocation">Enable Location</button>
                <p id="locationStatus" style="margin-top: 15px;"></p>
            </section>

            <!-- Event Section -->
            <section class="event-section fade-in">
                <div class="event-image">
                    <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/极市Images/Screenshot_20250831_072244_Gallery.jpg" alt="Bustani Gardens Event">
                </div>
                <div class="event-description">
                    <span class="exclusive极市-tag">EXCLUSIVE EVENT</span>
                    <h2>Bustani Gardens Masterclass Experience</h2>
                    <p>Join us for an exclusive culinary experience at Bustani Gardens, Red Hill. This is not just an event—it's a transformation for the top 0.00001% who understand that marketing excellence is the key to domination in any field.</p>
                    <p>Laansale101 and Exquisite Madiwa Flavors present a fusion of elite taste and marketing mastery. Learn how to capture attention, create desire, and command loyalty through sensory experience.</p>
                    <p>This is where the extraordinary is ordinary, and the exceptional is expected.</p>
                    <button class="btn">Reserve Your Spot</button>
                </div>
            </section>

            <!-- EMF Poster Section -->
            <section class="emf-poster fade-in">
                <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070939_Gallery.jpg" alt="EMF Feel Me More">
            </section>

            <!-- Special Offer Banner -->
            <div class="special-offer fade-in">
                <h3>⏰ Limited Time Offer! 🚀</h3>
                <p>Order in the first 20 minutes of any hour and get 10% OFF your entire order!</p>
                <p id="countdown" style="font-weight: bold; margin-top: 10px;"></p>
            </div>

            <!-- Drink Sizes Reference -->
            <section class="drink-sizes fade-in">
                <h3>Our Drink Sizes</h3>
                <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_071625_Gallery.jpg" alt="Drink Sizes Reference">
                <p style="margin-top: 15px;">Small (350ml) | Medium (500ml) | Large (750ml)</p>
            </section>

            <!-- Menu Section -->
            <section class="menu-section">
                <div class="menu-category fade-in">
                    <h3>FRISS & 'KAK!</h3>
                    <div class="menu-items">
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Classic Crunch</span>
                                <span class="item-price">450/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070743_Gallery.jpg" alt="Classic Crunch" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class极市="item-desc">FRIES + 10 PCS MISHIKAKI + CHEF'S SIGNATURE SAUCE</p>
                            <span class="limited-edition">Limited Edition</span>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="classic-crunch">-</button>
                                    <span class="quantity" data-item="classic-crunch">0</span>
                                    <button class="quantity-btn plus" data-item="classic-crunch">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="classic-crunch" data-price极市="450">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Grand Sultan</span>
                                <span class="item-price">550/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070759_Gallery.jpg" alt="Grand Sultan" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">MEGA FRIES LOADED WITH 15 PCS MISHIKAKI + SPECIAL SAUCE</p>
                            <p class="item-desc">EXTRA MISHIKAKI @100/- PER SKEWER</p>
                            <span class="limited-edition">Limited Edition</span>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="grand-sultan">-</button>
                                    <span class="quantity" data-item="grand-sultan">0</span>
                                    <button class="quantity-btn plus" data-item="grand-sultan">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="grand-sultan" data-price="550">Add to Cart</button>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="menu-category fade-in">
                    <h3>FRESH JUICE</h3>
                    <div class="menu-items">
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Tangy Passion</span>
                                <span class="item-price" id="price-tangy-passion">250/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070846_Gallery.jpg" alt="Tangy Passion" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Bold Passion, Pure Tropical Energy</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="tangy-passion" data-size="small" data-price="250">Small: 250/-</button>
                                <button class="size-btn" data-item="tangy-passion" data-size="medium" data-price="350">Medium: 350/-极市</button>
                                <button class="size-btn" data-item="tangy-passion" data-size="large" data-price="450">Large: 450/-</button>
                            </div>
                            <div class="item-controls">
                                <极市div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="tangy-passion">-</button>
                                    <span class="quantity" data-item="tangy-passion">0</span>
                                    <button class="quantity-btn plus" data-item="tangy-passion">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="tangy-passion" data-price="250">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Mango Rush</span>
                                <span class="item-price" id="price-mango-rush">250/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070846_Gallery.jpg" alt="Mango Rush" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Thick, Juicy, Naturally Sweet</p>
                            <div class="size-options">
                                <button class="size-btn active极市" data-item="mango-rush" data-size="small" data-price极市="250">Small: 250/-</button>
                                <button class="size-btn" data-item="mango-rush" data-size="medium" data-price="350">Medium: 350/-</button>
                                <button class="size-btn" data-item="mango-rush" data-size="large" data-price="450">Large: 450/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="mango-rush">-</button>
                                    <span class="quantity" data-item="mango-rush">0</span>
                                    <button class="quantity-btn plus" data-item="mango-rush">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="mango-rush" data-price="250">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Le' Pineapple De' Mint</span>
                                <span class="item-price" id="price-pineapple-mint">250/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070851_Gallery.jpg" alt="Le Pineapple De Mint" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Altuty Breeze, Pineapple Squeeze</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="pineapple-mint" data-size="small" data-price="250">Small: 250/-</button>
                                <button class="size-btn" data-item="pineapple-mint" data-size="medium" data-price="350">Medium: 350/-</button>
                                <button class="size-btn" data-item="pineapple-mint" data-size="large" data-price="450">Large: 450/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="pineapple-mint">-</button>
                                    <span class="quantity" data-item="pineapple-mint">0</span>
                                    <button class="quantity-btn plus" data-item="pineapple-mint">-</button>
                                </div>
                                <button class="btn add-to-cart" data-item="pineapple-m极市int" data-price="250">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Tropical Mix</span>
                                <span class="item-price" id="price-tropical-mix">250/-</极市span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_极市20250831_070856_Gallery.jpg" alt="Tropical Mix" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">All-in-one island infusion</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="tropical-mix" data-size="small" data-price="250">Small: 250/-</button>
                                <button class="size-btn" data-item="tropical-mix" data-size="medium" data-price="350">Medium: 350/-</button>
                                <button class="size-btn" data-item="tropical-mix" data-size="large" data-price="450">Large: 450/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="tropical-mix">-</button>
                                    <span class="quantity" data-item="tropical-mix">0</span>
                                    <button class="quantity-btn plus" data-item="tropical-mix">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="tropical-mix" data-price="250">Add to Cart</button>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="menu-category fade-in">
                    <h3>MAGIC MOJITOS</h3>
                    <div class="menu-items">
                        <div class="menu-item">
                            <div class="极市item-header">
                                <span class="item-name">Blue Lagoon</span>
                                <span class="item-price" id="price-blue-lagoon">300/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070907_Gallery.jpg" alt="Blue Lagoon" style极市="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Tropical Citrus Wave, Blue Ocean</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="blue-lagoon" data-size="small" data-price="300">Small: 300/-</button>
                                <button class="size-btn" data-item="blue-lagoon" data-size="medium" data-price="400">Medium: 400/-</button>
                                <button class="size-btn" data-item="blue-lagoon" data-size="large" data-price="500">Large: 500/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="blue-lagoon">-</button>
                                    <span class="quantity" data-item="blue-lagoon">0</span>
                                    <button class="quantity-btn plus" data-item="blue-lagoon">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="blue-lagoon" data-price="300">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Red Flash</span>
                                <span class="item-price" id="price-red-flash">300/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales极市999/Laan101emf/main/Images/Screenshot_20250831_070912_Gallery.jpg" alt="Red Flash" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Bold strawberry heat meets cool mint</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="red-flash" data-size="small" data-price="300">Small: 300/-</button>
                                <button class="size-btn" data-item="red-flash" data-size="medium" data-price="400">Medium: 400/-</button>
                                <button class="size-btn" data-item="red-flash" data-size="large" data-price="500">Large: 500/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data极市-item="red-flash">-</button>
                                    <span class="quantity" data-item="red-flash">0极市</span>
                                    <button class="quantity-btn plus" data-item="red-flash">+</button>
                                </div>
                                <button class极市="btn add-to-cart" data-item="red-flash" data-price="300">Add to Cart</button>
                            </极市div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Berry Breeze极市</span>
                                <span class="item-price" id="price-berry-breeze">300/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070921_Gallery.jpg" alt="Berry Breeze" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Smooth berry chill, island style</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="berry-breeze" data-size="small" data-price="300">Small: 300/-</button>
                                <button class="size-btn" data-item="berry-breeze" data-size="medium" data-price="400">Medium: 400/-</button>
                                <button class="size-btn" data-item="berry-breeze" data-size="large" data-price="500">Large: 500/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="berry-breeze">-</button>
                                    <span class="quantity" data-item="berry-breeze">0</span>
                                    <button class="quantity-btn plus" data-item="berry-breeze">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="berry-breeze" data-price="300">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Ginger Gold</span>
                                <span class="item-price" id="price-ginger-gold">300/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070926_Gallery.jpg" alt="Ginger Gold" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Golden spice with honeyed flow</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="ginger-gold" data-size="small" data-price="300极市">Small: 300/-</button>
                                <button class="size-btn" data-item="ginger-gold" data-size="medium" data-price="400">Medium: 400/-</button>
                                <button class="size-btn" data-item="ginger-gold" data-size="large" data-price="500">Large: 500/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="ginger-gold">-</button>
                                    <span class="quantity" data-item="ginger-gold">0</span>
                                    <button class="quantity-btn plus" data-item="ginger-gold">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="ginger-gold" data-price="300">Add to Cart</button>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Checkout Form -->
            <section class="checkout-form" id="checkout-form">
                <h3>Complete Your Order</h3>
                <div class="form-group">
                    <label for="name">Full Name</label>
                    <input type="text" id="name" required>
                </div>
                <极市div class="form-group">
                    <label for="phone">Phone Number</label>
                    <input type="tel" id="phone" required>
                </div>
                <div class="form-group">
                    <label for="dressing">Dressing Description (Optional)</label>
                    <textarea id="dressing" rows="3"></textarea>
                </div>
                <div class="form-group">
                    <label for="location">Delivery Location</极市label>
                    <input type="text" id="delivery-location" readonly>
                    <small>If the location is not accurate, please describe your location below</small>
                </div>
                <div class="form-group">
                    <label for="location-details">Location Details (If needed)</label>
                    <textarea id="location-details" rows="2"></textarea>
                </div>
                
                <!-- Payment Information -->
                <div class="payment-info">
                    <h极市4>Payment Method</h4>
                    <p>We accept Lipa na M-Pesa</p>
                    <p><strong>Paybill:</strong> 542542</p>
                    <p><strong>Account Number:</strong> 786867</p>
                    <p>Please complete payment before placing your order</p>
                </div>
                
                <button class="checkout-btn" id="place-order">Place Order via WhatsApp</button>
            </section>
        </div>

        <!-- Floating Cart -->
        <div class="floating-cart cart-hidden" id="floating-cart">
            <div class极市="cart-header">
                <h3>Your Order</h3>
                <span id="cart-count">0 items</span>
            </div>
            <div class="cart-items" id="cart-items">
                <p style="text-align: center; padding: 20px;">Your cart is empty</p>
            </div>
            <div class="cart-total">
                <span>Total:</span>
                <span id="cart-total">0/-</span>
            </div>
            <button class="checkout-btn" id="checkout-btn">Proceed to Checkout</button>
        </div>

        <!-- Cart Toggle Button -->
        <div class="cart-toggle" id="cart-toggle">
            <i class="fas fa-shopping-cart"></i>
            <span class="cart-badge" id="cart-badge">0</span>
        </div>

        <!-- WhatsApp Chat -->
        <a href="https://wa.me/254115030726" class="whatsapp-chat" target="_blank">
            <i class="fab fa-whatsapp"></i>
        </a>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-about">
                    <h3>About Laansales101</h3>
                    <p>Laansales101 was born from a deep understanding of the challenges that vendors and event-goers face. What if there was a way to merge convenience with luxury, to transform an ordinary event into an extraordinary experience? That vision led to the creation of Laansales101—a cutting-edge platform designed to make ordering seamless, effortless, and uniquely personal for every event-goer.</p>
                </div>
                <div class="footer-contact">
                    <h3>Contact Us</h3>
                    <p><极市i class="fas fa-envelope"></i> emflavorsales@gmail.com</p>
                    <p><i class="fas fa-phone"></i> +254 115 030 726</p>
                    <p><i class="fab fa-whatsapp"></i> WhatsApp: +254 115 030 726</p>
                </div>
            </div>
            <div class="footer-logo">
                <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070816_Gallery.jpg" alt="Laansale Logo">
            </div>
            <div class="footer-bottom">
                <p>&copy; 2025 Laansales101. All Rights Reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Initialize cart
        let cart = [];
        let userLocation = null;
        
        // DOM Elements
        const enableLocationBtn = document.getElementById('enableLocation');
        const locationStatus = document.getElementById('locationStatus');
        const checkoutBtn = document.getElementById('checkout-btn');
        const checkoutForm = document.getElementById('checkout-form');
        const placeOrderBtn = document.getElementById('place-order');
        const deliveryLocation = document.getElementById('delivery-location');
        const countdownEl = document.getElementById('countdown');
        const floatingCart = document.getElementById('floating-cart');
        const cartToggle = document.getElementById('cart-toggle');
        const cartBadge = document.getElementById('cart-badge');
        
        // Cart toggle functionality
        let cartVisible = false;
        
        cartToggle.addEventListener('click', () => {
            cartVisible = !cartVisible;
            if (cartVisible) {
                floatingCart.classList.remove('cart-hidden');
            } else {
                floatingCart.classList.add('cart-hidden');
            }
        });
        
        // Enable location
        enableLocationBtn.addEventListener('click', () => {
            if (navigator.geolocation) {
                navigator.geolocation.getCurrentPosition(
                    position => {
                        userLocation = position;
                        const { latitude, longitude } = position.coords;
                        locationStatus.innerHTML = `Location enabled! Latitude: ${latitude.toFixed(6)}, Longitude: ${longitude.toFixed(6)}`;
                        locationStatus.style.color = '#10b981';
                        deliveryLocation.value = `${latitude.toFixed(6)}, ${longitude极市.toFixed(6)}`;
                        
                        // Try to get address from coordinates
                        getAddressFromCoords(latitude, longitude);
                    },
                    error => {
                        locationStatus.innerHTML = 'Unable to retrieve location. Please describe your location in the checkout form.';
                        locationStatus.style.color = '#ef4444';
                        deliveryLocation.value = 'Location not available. Please describe below.';
                    }
                );
            } else {
                locationStatus.innerHTML = 'Geolocation is not supported by this browser. Please describe your location in the checkout form.';
                locationStatus.style.color = '#ef4444';
                deliveryLocation.value = 'Geolocation not supported. Please describe below.';
            }
        });
        
        // Function to get address from coordinates
        function getAddressFromCoords(lat, lng) {
            // Using Nominatim (OpenStreetMap) for reverse geocoding
            fetch(`https://nominatim.openstreetmap.org/reverse?format=json&lat=${lat}&lon=${lng}`)
                .then(response => response.json())
                .then(data => {
                    if (data && data.display_name) {
                        deliveryLocation.value = data.display_name;
                    }
                })
                .catch(error => {
                    console.error('Error getting address:', error);
                });
        }
        
        // Size selection for drinks
        document.querySelectorAll('.size-btn').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const size = button.getAttribute('data-size');
                const price = button.getAttribute('data-price');
                
                // Remove active class from all buttons in this group
                button.parentNode.querySelectorAll('.size-btn').forEach(btn => {
                    btn.classList.remove('active');
                });
                
                // Add active class to clicked button
                button.classList.add('active');
                
                // Update price display
                document.getElementById(`price-${item}`).textContent = `${price}/-`;
                
                // Update add to cart button data-price
                const addButton = button.closest('.menu-item').querySelector('.add极市-to-cart');
                addButton.setAttribute('data-price', price);
            });
        });
        
        // Quantity controls
        document.querySelectorAll('.quantity-btn').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const quantityEl = document.querySelector(`.quantity[data-item="${item}"]`);
                let quantity = parseInt(quantityEl.textContent);
                
                if (button.classList.contains('plus')) {
                    quantity++;
                } else if (button.classList.contains('minus') && quantity > 0) {
                    quantity--;
                }
                
                quantityEl.textContent = quantity;
            });
        });
        
        // Add to cart
        document.querySelectorAll('.add-to-cart').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const price = parseInt(button.getAttribute('data-price'));
                const quantity = parseInt(document.querySelector(`.quantity[data-item="${item}"]`).textContent);
                
                if (quantity === 0) return;
                
                // Get selected size for drinks
                let size = null;
                const sizeBtn = button.closest('.menu-item').querySelector('.size-btn.active');
                if (sizeBtn) {
                    size = sizeBtn.getAttribute('data-size');
                }
                
                // Check if item already in cart
                const existingItemIndex = cart.findIndex(cartItem => 
                    cartItem.name === item && cartItem.size === size
                );
                
                if (existingItemIndex !== -1) {
                    cart[existingItemIndex].quantity += quantity;
                } else {
                    cart.push({
                        name: item,
                        price: price,
                        quantity: quantity,
                        size: size
                    });
                }
                
                updateCart();
                
                // Reset quantity
                document.querySelector(`.quantity[data-item="${item}"]`).textContent = '0';
                
                // Show cart
                floatingCart.classList.remove('cart-hidden');
                cartVisible = true;
            });
        });
        
        // Update cart
        function updateCart() {
            const cartItems = document.getElementById('cart-items');
            const cartCount = document.getElementById('cart-count');
            const cartTotal = document.getElementById('cart-total');
            
            // Clear cart items
            cartItems.innerHTML = '';
            
            if (cart.length === 0) {
                cartItems.innerHTML = '<p style="text-align: center; padding: 20px;">Your cart is empty</p>';
                cartCount.textContent = '0 items';
                cartTotal.textContent = '0/-';
                cartBadge.textContent = '0';
                return;
            }
            
            let total = 0;
            let item极市Count = 0;
            
            cart.forEach((item, index) => {
                const itemTotal = item.price * item.quantity;
                total += itemTotal;
                itemCount += item.quantity;
                
                const cartItemEl = document.createElement('div');
                cartItemEl.className = 'cart-item';
                
                let sizeInfo = '';
                if (item.size) {
                    sizeInfo = ` (${item.size})`;
                }
                
                cartItemEl.innerHTML = `
                    <div class="cart-item-info">
                        <div>${formatItemName(item.name)}${sizeInfo}</div>
                        <div>${item.price}/- x ${item.quantity}</div>
                    </div>
                    <div class="cart-item-controls">
                        <span>${itemTotal}/-</span>
                        <button class="remove-btn" data-index="${index}">
                            <i class="fas fa-trash"></i>
                        </button>
                    </div>
                `;
                
                cartItems.appendChild(cartItemEl);
            });
            
            cartCount.textContent = `${itemCount} ${itemCount === 1 ? 'item' : 'items'}`;
            cartTotal.textContent = `${total}/-`;
            cartBadge.textContent = itemCount;
            
            // Add event listeners to remove buttons
            document.querySelectorAll('.remove-btn').forEach(button => {
                button.addEventListener('click', () => {
                    const index = parseInt(button.getAttribute('data-index'));
                    cart.splice(index, 1);
                    updateCart();
                });
            });
        }
        
        // Format item name for display
        function formatItemName(name) {
            return name.split('-')
                .map(word => word.charAt(0).toUpperCase() + word.slice(1))
                .join(' ');
        }
        
        // Checkout button
        checkoutBtn.addEventListener('click', () => {
            if (cart.length === 0) {
                alert('Your cart is empty. Please add items before checkout.');
                return;
            }
            
            checkoutForm.style.display = 'block';
            checkoutForm.scrollIntoView({ behavior: 'smooth' });
        });
        
        // Place order
        placeOrderBtn.addEventListener('click', () => {
            const name = document.getElementById('name').value;
            const phone = document.getElementById('phone').value;
            
            if (!name || !phone) {
                alert('Please fill in all required fields.');
                return;
            }
            
            // Create order summary
            let orderSummary = `*NEW ORDER FROM EXQUISITE MADIWA FLAVORS WEBSITE*\n\n`;
            orderSummary += `*Customer Name:* ${name}\n`;
            orderSummary += `*Phone:* ${phone}\n`;
            
            // Add location information
            const locationDetails = document.getElementById('location-details').value;
            if (deliveryLocation.value && deliveryLocation.value !== 'Location not available. Please describe below.') {
                orderSummary += `*Location:* ${deliveryLocation.value}\n`;
            }
            if (locationDetails) {
                orderSummary += `*Location Details:* ${locationDetails}\n`;
            }
            
            orderSummary += `\n*Order Details:*\n`;
            
            cart.forEach(item => {
                let sizeInfo = '';
                if (item.size) {
                    sizeInfo = ` (${item.size})`;
                }
                orderSummary += `- ${formatItemName(item.name)}${sizeInfo} x ${item.quantity} = ${item.price * item.quantity}/-\n`;
            });
            
            orderSummary += `\n*Total: ${cart.reduce((total, item) => total + (item.price * item.quantity), 0)}/-*\n\n`;
            
            const dressing = document.getElementById('dressing').value;
极市           if (dressing) {
                orderSummary += `*Dressing Instructions:* ${dressing}\n`;
            }
            
            orderSummary += `\n*Payment Method:* Lipa na M-Pesa\n`;
            orderSummary += `*Paybill:* 542542\n`;
            orderSummary += `*Account Number:* 786867\n`;
            
            // Encode for WhatsApp URL
            const encodedMessage = encodeURIComponent(orderSummary);
            const whatsappURL = `https://wa.me/254115030726极市?text=${encodedMessage}`;
            
            // Open WhatsApp
            window.open(whatsappURL, '_blank');
            
            // Reset cart and form
            cart = [];
            updateCart();
            checkoutForm.style.display = 'none';
            document.getElementById('name').value = '';
            document.getElementById('phone').value = '';
            document.getElementById('dressing').value = '';
            document.getElementById('location-details').value = '';
            
            alert('Your order has been placed! You will be redirected to WhatsApp to confirm.');
        });
        
        // Countdown timer for special offer
        function updateCountdown() {
            const now = new Date();
            const minutes = now.getMinutes();
            const seconds = now.getSeconds();
            
            if (minutes < 20) {
                const timeLeft = 20 - minutes;
                const secsLeft = 60 - seconds;
                countdownEl.textContent = `Offer ends in: ${timeLeft} min ${secsLeft} sec`;
            } else {
                const nextHour = new Date(now);
                nextHour.setHours(nextHour.getHours() + 1);
                nextHour.setMinutes(0);
                nextHour.setSeconds(0);
                
                const diff = nextHour - now;
                const minsLeft = Math.floor(diff / 60000);
                const secsLeft = Math.floor((diff % 60000) / 1000);
                
                countdown极市El.textContent = `Next offer in: ${minsLeft} min ${secsLeft} sec`;
            }
        }
        
        setInterval(updateCountdown, 1000);
        updateCountdown();
        
        // Add fade-in animation to elements when they come into view
        const fadeElements = document.querySelectorAll('.fade-in');
        
        const fadeInObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animation = 'fadeIn 1s ease forwards';
                    fadeInObserver.unobserve(entry.target);
                }
            });
        }, { threshold: 0.1 });
        
        fadeElements.forEach(element => {
            fadeInObserver.observe(element);
        });
    </script>
</body>
</html>: #f8f8f8;
            --dark-text: #1e293b;
            --transition: all 0.4s cubic-bezier(0.175, 0.885, 0.32, 1.275);
        }
        
        body {
            background: linear-gradient(135deg, var(--dark-blue) 0%, #1e3a8a 100%);
            color: var(--light-text);
            line-height: 1.6;
            padding-bottom: 80px;
            font-family: 'Poppins', sans-serif;
            overflow-x: hidden;
        }
        
        .container {
            width: 100%;
            max-width: 1200px;
            margin: 0 auto;
            padding: 20px;
        }
        
        /* Header Styles - COMPACT & ELEGANT */
        .main-header {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            display: flex;
            justify-content: center;
            align-items: center;
            padding: 5px 0;
            background: rgba(10, 25, 47, 0.97);
            backdrop-filter: blur(10px);
            z-index: 10000;
            transition: var(--transition);
            box-shadow: 0 2px 8px rgba(0, 0, 0, 0.2);
            border-bottom: 1px solid var(--gold);
            height: 50px;
        }
        
        .header-hidden {
            transform: translateY(-100%);
            opacity: 0;
        }
        
        .logo-container {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .logo {
            width: 100px;
            height: auto;
            transition: var(--transition);
        }
        
        .tagline {
            display: none; /* Hidden for compact header */
        }
        
        /* Main Content */
        .main-content {
            padding-top: 70px;
        }
        
        /* Rest of the CSS remains the same as before */
        .location-prompt {
            background: rgba(14, 165, 233, 0.15);
            padding: 25px;
            border-radius: 15px;
            text-align: center;
            margin-bottom: 40px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        /* ... (rest of your CSS styles) ... */
        
    </style>
</head>
<body>
    <div class="container">
        <!-- Header with Logo -->
        <header class="main-header" id="main-header">
            <div class="logo-container">
                <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070816_Gallery.jpg" alt="Laansale Logo" class="logo">
            </div>
        </header>

        <div class="main-content">
            <!-- Your content here -->
            <section class="location-prompt fade-in">
                <h2><i class="fas fa-location-dot"></i> Enable Your Location</h2>
                <p>To serve you better and provide accurate delivery, please enable location services</p>
                <button class="btn" id="enableLocation">Enable Location</button>
                <p id="locationStatus" style="margin-top: 15px;"></p>
            </section>
            
            <!-- Rest of your content -->
        </div>
        
        <!-- Rest of your HTML -->
    </div>

    <script>
        // Header scroll behavior
        let lastScrollTop = 0;
        const mainHeader = document.getElementById('main-header');
        
        window.addEventListener('scroll', function() {
            let scrollTop = window.pageYOffset || document.documentElement.scrollTop;
            
            if (scrollTop > lastScrollTop && scrollTop > 50) {
                // Scrolling down
                mainHeader.classList.add('header-hidden');
            } else {
                // Scrolling up
                mainHeader.classList.remove('header-hidden');
            }
            
            lastScrollTop = scrollTop;
        });
        
        // Rest of your JavaScript
    </script>
</body>
</html>
        
        .logo-container {
            display: flex;
            flex-direction: column;
            align-items: center;
        }
        
        .logo {
            width: 120px;
            height: auto;
            transition: var(--transition);
        }
        
        .logo:hover {
            transform: scale(1.05);
        }
        
        .tagline {
            font-style: italic;
            color: var(--gold);
            margin-top: 5px;
            font-size: 0.9rem;
            font-family: 'Playfair Display', serif;
        }
        
        /* Footer Styles */
        footer {
            background: var(--dark-blue);
            padding: 60px 0 30px;
            margin-top: 60px;
            border-top: 2px solid var(--gold);
            position: relative;
        }
        
        .footer-content {
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            gap: 30px;
        }
        
        .footer-about {
            flex: 2;
            min-width: 300px;
        }
        
        .footer-about h3 {
            color: var(--gold);
            margin-bottom: 15px;
            font-size: 1.5rem;
            font-family: 'Playfair Display', serif;
        }
        
        .footer-about p {
            margin-bottom: 15px;
            line-height: 1.8;
            font-size: 0.95rem;
        }
        
        .footer-contact {
            flex: 1;
            min-width: 250px;
        }
        
        .footer-contact h3 {
            color: var(--gold);
            margin-bottom: 15px;
            font-size: 1.5rem;
            font-family: 'Playfair Display', serif;
        }
        
        .footer-contact p {
            margin-bottom: 10px;
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .footer-logo {
            text-align: center;
            margin-top: 30px;
        }
        
        .footer-logo img {
            width: 120px;
            opacity: 0.9;
        }
        
        .footer-bottom {
            text-align: center;
            margin-top: 40px;
            padding-top: 20px;
            border-top: 1px solid rgba(255, 255, 255, 0.1);
            font-size: 0.9rem;
        }
        
        /* Main Content */
        .main-content {
            padding-top: 90px;
        }
        
        .location-prompt {
            background: rgba(14, 165, 233, 0.15);
            padding: 25px;
            border-radius: 15px;
            text-align: center;
            margin-bottom: 40px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        
        .location-prompt h2 {
            margin-bottom: 15px;
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            font-family: 'Playfair Display', serif;
        }
        
        .btn {
            background: var(--gold);
            color: white;
            border: none;
            padding: 14px 30px;
            border-radius: 50px;
            cursor: pointer;
            font-weight: 600;
            transition: var(--transition);
            display: inline-block;
            margin-top: 15px;
            font-size: 1rem;
            letter-spacing: 0.5px;
            box-shadow: 0 4px 10px rgba(245, 158, 11, 0.3);
        }
        
        .btn:hover {
            background: #d97706;
            transform: translateY(-3px);
            box-shadow: 0 6px 15px rgba(0, 0, 0, 0.2);
        }
        
        .event-section {
            display: flex;
            flex-wrap: wrap;
            gap: 30px;
            margin-bottom: 50px;
            align-items: center;
        }
        
        .event-image {
            flex: 1;
            min-width: 300px;
            border-radius: 15px;
            overflow: hidden;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            transition: var(--transition);
        }
        
        .event-image:hover {
            transform: translateY(-5px);
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.4);
        }
        
        .event-image img {
            width: 100%;
            height: auto;
            display: block;
            transition: var(--transition);
        }
        
        .event-image:hover img {
            transform: scale(1.03);
        }
        
        .event-description {
            flex: 2;
            min-width: 300px;
            background: var(--light-bg);
            padding: 30px;
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .event-description h2 {
            color: var(--primary-blue);
            margin-bottom: 20px;
            font-size: 32px;
            font-family: 'Playfair Display', serif;
        }
        
        .event-description p {
            margin-bottom: 20px;
            font-size: 16px;
            line-height: 1.8;
        }
        
        .exclusive-tag {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            color: white;
            padding: 8px 20px;
            border-radius: 20px;
            font-size: 14px;
            font-weight: 600;
            display: inline-block;
            margin-bottom: 20px;
            letter-spacing: 0.5px;
        }
        
        .emf-poster {
            text-align: center;
            margin: 50px 0;
        }
        
        .emf-poster img {
            max-width: 100%;
            border-radius: 15px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            transition: var(--transition);
        }
        
        .emf-poster img:hover {
            transform: scale(1.02);
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.4);
        }
        
        .special-offer {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            padding: 20px;
            border-radius: 15px;
            text-align: center;
            margin: 30px 0;
            animation: pulse 2s infinite;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }
        
        .special-offer h3 {
            font-size: 1.5rem;
            margin-bottom: 10px;
        }
        
        .menu-section {
            margin: 50px 0;
        }
        
        .menu-category {
            margin-bottom: 50px;
        }
        
        .menu-category h3 {
            color: var(--primary-blue);
            border-bottom: 2px solid var(--primary-blue);
            padding-bottom: 15px;
            margin-bottom: 30px;
            font-size: 28px;
            font-family: 'Playfair Display', serif;
        }
        
        .menu-items {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(320px, 1fr));
            gap: 25px;
        }
        
        .menu-item {
            background: var(--light-bg);
            border-radius: 15px;
            padding: 25px;
            transition: var(--transition);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
            position: relative;
            overflow: hidden;
        }
        
        .menu-item::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: linear-gradient(135deg, rgba(12, 77, 162, 0.1), rgba(245, 158, 11, 0.1));
            z-index: -1;
            opacity: 0;
            transition: var(--transition);
        }
        
        .menu-item:hover {
            transform: translateY(-8px);
            box-shadow: 0 12px 30px rgba(0, 0, 0, 0.2);
        }
        
        .menu-item:hover::before {
            opacity: 1;
        }
        
        .item-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 15px;
        }
        
        .item-name {
            font-weight: 700;
            font-size: 20px;
            color: var(--light-text);
            font-family: 'Playfair Display', serif;
        }
        
        .item-price {
            color: var(--gold);
            font-weight: 800;
            font-size: 22px;
        }
        
        .item-desc {
            color: #cbd5e1;
            font-size: 15px;
            margin-bottom: 20px;
            line-height: 1.6;
        }
        
        .size-options {
            display: flex;
            gap: 10px;
            margin-bottom: 20px;
            flex-wrap: wrap;
        }
        
        .size-btn {
            padding: 8px 15px;
            border-radius: 20px;
            border: 1px solid var(--primary-blue);
            background: transparent;
            color: var(--light-text);
            cursor: pointer;
            font-size: 13px;
            transition: var(--transition);
        }
        
        .size-btn.active {
            background: var(--primary-blue);
            color: white;
            box-shadow: 0 4px 10px rgba(12, 77, 162, 0.3);
        }
        
        .item-controls {
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        
        .quantity-controls {
            display: flex;
            align-items: center;
            gap: 12px;
        }
        
        .quantity-btn {
            background: var(--primary-blue);
            color: white;
            border: none;
            width: 35px;
            height: 35px;
            border-radius: 50%;
            cursor: pointer;
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
            font-weight: bold;
        }
        
        .quantity-btn:hover {
            background: #0a3d80;
            transform: scale(1.1);
        }
        
        .quantity {
            font-weight: 700;
            width: 35px;
            text-align: center;
            font-size: 18px;
        }
        
        .limited-edition {
            background: linear-gradient(135deg, var(--gold), #ef4444);
            color: white;
            padding: 5px 15px;
            border-radius: 15px;
            font-size: 13px;
            font-weight: 600;
            display: inline-block;
            margin-top: 15px;
            letter-spacing: 0.5px;
        }
        
        /* Drink Sizes Section */
        .drink-sizes {
            text-align: center;
            margin: 50px 0;
            padding: 30px;
            background: var(--light-bg);
            border-radius: 15px;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .drink-sizes h3 {
            color: var(--primary-blue);
            margin-bottom: 25px;
            font-size: 28px;
            font-family: 'Playfair Display', serif;
        }
        
        .drink-sizes img {
            max-width: 100%;
            border-radius: 15px;
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.3);
            transition: var(--transition);
        }
        
        .drink-sizes img:hover {
            transform: scale(1.02);
        }
        
        /* Floating Cart */
        .floating-cart {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: var(--light-bg);
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            border-radius: 15px;
            padding: 20px;
            width: 350px;
            box-shadow: 0 10px 30px rgba(0, 0, 0, 0.3);
            z-index: 1000;
            max-height: 450px;
            overflow-y: auto;
            transition: var(--transition);
            transform: translateX(0);
        }
        
        .cart-hidden {
            transform: translateX(400px);
        }
        
        .cart-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 20px;
            padding-bottom: 15px;
            border-bottom: 1px solid rgba(255, 255, 255, 0.1);
        }
        
        .cart-header h3 {
            font-family: 'Playfair Display', serif;
            color: var(--gold);
        }
        
        .cart-items {
            max-height: 250px;
            overflow-y: auto;
            margin-bottom: 20px;
        }
        
        .cart-item {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 12px 0;
            border-bottom: 1px solid rgba(255, 255, 255, 0.05);
            font-size: 15px;
        }
        
        .cart-item-info {
            flex: 2;
        }
        
        .cart-item-controls {
            display: flex;
            align-items: center;
            gap: 10px;
        }
        
        .remove-btn {
            color: #ef4444;
            background: none;
            border: none;
            cursor: pointer;
            font-size: 16px;
            transition: var(--transition);
        }
        
        .remove-btn:hover {
            transform: scale(1.2);
        }
        
        .cart-total {
            display: flex;
            justify-content: space-between;
            align-items: center;
            font-weight: 800;
            font-size: 20px;
            padding-top: 15px;
            border-top: 2px solid rgba(255, 255, 255, 0.1);
            color: var(--gold);
        }
        
        .checkout-btn {
            width: 100%;
            padding: 15px;
            background: linear-gradient(135deg, #10b981, #059669);
            color: white;
            border: none;
            border-radius: 50px;
            font-weight: 700;
            font-size: 16px;
            cursor: pointer;
            transition: var(--transition);
            margin-top: 20px;
            letter-spacing: 0.5px;
            box-shadow: 0 5px 15px rgba(16, 185, 129, 0.3);
        }
        
        .checkout-btn:hover {
            transform: translateY(-3px);
            box-shadow: 0 8px 20px rgba(16, 185, 129, 0.4);
        }
        
        .checkout-form {
            background: var(--light-bg);
            border-radius: 15px;
            padding: 30px;
            margin-top: 50px;
            display: none;
            backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 255, 255, 0.1);
            box-shadow: 0 8px 25px rgba(0, 0, 0, 0.2);
        }
        
        .checkout-form h3 {
            color: var(--gold);
            margin-bottom: 25px;
            font-size: 28px;
            font-family: 'Playfair Display', serif;
            text-align: center;
        }
        
        .form-group {
            margin-bottom: 25px;
        }
        
        .form-group label {
            display: block;
            margin-bottom: 10px;
            font-weight: 600;
            font-size: 16px;
        }
        
        .form-group input, .form-group textarea, .form-group select {
            width: 100%;
            padding: 15px 20px;
            border-radius: 10px;
            border: 1px solid rgba(255, 255, 255, 0.1);
            background: rgba(255, 255, 255, 0.1);
            color: white;
            font-size: 16px;
            transition: var(--transition);
        }
        
        .form-group input:focus, .form-group textarea:focus, .form-group select:focus {
            outline: none;
            border-color: var(--primary-blue);
            box-shadow: 0 0 0 2px rgba(12, 77, 162, 0.3);
        }
        
        .payment-info {
            background: rgba(14, 165, 233, 0.1);
            padding: 20px;
            border-radius: 10px;
            margin: 25px 0;
            border-left: 4px solid var(--primary-blue);
        }
        
        .payment-info h4 {
            color: var(--gold);
            margin-bottom: 15px;
            font-size: 20px;
            font-family: 'Playfair Display', serif;
        }
        
        .payment-info p {
            margin-bottom: 10px;
        }
        
        .whatsapp-chat {
            position: fixed;
            bottom: 110px;
            right: 30px;
            background: #25D366;
            color: white;
            width: 65px;
            height: 65px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 30px;
            box-shadow: 0 6px 20px rgba(37, 211, 102, 0.4);
            z-index: 1000;
            transition: var(--transition);
        }
        
        .whatsapp-chat:hover {
            transform: scale(1.1);
            box-shadow: 0 8px 25px rgba(37, 211, 102, 0.5);
        }
        
        .cart-toggle {
            position: fixed;
            bottom: 30px;
            right: 30px;
            background: var(--gold);
            color: white;
            width: 65px;
            height: 65px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 26px;
            box-shadow: 0 6px 20px rgba(245, 158, 11, 0.4);
            z-index: 1000;
            transition: var(--transition);
            cursor: pointer;
        }
        
        .cart-toggle:hover {
            transform: scale(1.1);
            box-shadow: 0 8px极市25px rgba(245, 158, 11, 0.5);
        }
        
        .cart-badge {
            position: absolute;
            top: -5px;
            right: -5px;
            background: #ef4444;
            color: white;
            width: 26px;
            height: 26px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            font-size: 13px;
            font-weight: 700;
            box-shadow: 0 2px 8px rgba(239, 68, 68, 0.3);
        }
        
        @keyframes pulse {
            0% { transform: scale(1); }
            50% { transform: scale(1.02); }
            100% { transform: scale(1); }
        }
        
        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }
        
        .fade-in {
            animation: fadeIn 1s ease forwards;
        }
        
        @media (max-width: 1024px) {
            .menu-items {
                grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
            }
        }
        
        @media (max-width: 768px) {
            .event-section {
                flex-direction: column;
            }
            
            .menu-items {
                grid-template-columns: 1fr;
            }
            
            .floating-cart {
                width: 90%;
                left: 5%;
                right: 5%;
                bottom: 100px;
            }
            
            .footer-content {
                flex-direction: column;
            }
            
            .cart-toggle {
                bottom: 20px;
                right: 20px;
            }
            
            .whatsapp-chat {
                bottom: 100px;
                right: 20px;
            }
            
            .main-header {
                padding: 8px 0;
                height: 60px;
            }
            
            .logo {
                width: 100px;
            }
            
            .tagline {
                font-size: 0.8rem;
            }
            
            .main-content {
                padding-top: 80px;
            }
        }
        
        @media (max-width: 480px) {
            .container {
                padding: 15px;
            }
            
            .btn {
                padding: 12px 25px;
                font-size: 0.9rem;
            }
            
            .event-description {
                padding: 20px;
            }
            
            .menu-item {
                padding: 20px;
            }
            
            .item-name {
                font-size: 18px;
            }
            
            .item-price {
                font-size: 20px;
            }
            
            .main-header {
                height: 55px;
            }
            
            .logo {
                width: 90px;
            }
            
            .tagline {
                display: none;
            }
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Header with Logo -->
        <header class="main-header" id="main-header">
            <div class="logo-container">
                <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070816_Gallery.jpg" alt="Laansale Logo" class="logo">
                <div class="tagline">Premium Culinary Experiences</div>
            </div>
        </header>

        <div class="main-content">
            <!-- Location Prompt Section -->
            <section class="location-prompt fade-in">
                <h2><i class="fas fa-location-dot"></i> Enable Your Location</h2>
                <p>To serve you better and provide accurate delivery, please enable location services</p>
                <button class="btn" id="enableLocation">Enable Location</button>
                <p id="locationStatus" style="margin-top: 15px;"></p>
            </section>

            <!-- Event Section -->
            <section class="event-section fade-in">
                <div class="event-image">
                    <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_072244_Gallery.jpg" alt="Bustani Gardens Event">
                </div>
                <div class="event-description">
                    <span class="exclusive-tag">EXCLUSIVE EVENT</span>
                    <h2>Bustani Gardens Masterclass Experience</h2>
                    <p>Join us for an exclusive culinary experience at Bustani Gardens, Red Hill. This is not just an event—it's a transformation for the top 0.00001% who understand that marketing excellence is the key to domination in any field.</p>
                    <p>Laansale101 and Exquisite Madiwa Flavors present a fusion of elite taste and marketing mastery. Learn how to capture attention, create desire, and command loyalty through sensory experience.</p>
                    <p>This is where the extraordinary is ordinary, and the exceptional is expected.</p>
                    <button class="btn">Reserve Your Spot</button>
                </div>
            </section>

            <!-- EMF Poster Section -->
            <section class="emf-poster fade-in">
                <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070939_Gallery.jpg" alt="EMF Feel Me More">
            </section>

            <!-- Special Offer Banner -->
            <div class="special-offer fade-in">
                <h3>⏰ Limited Time Offer! 🚀</h3>
                <p>Order in the first 20 minutes of any hour and get 10% OFF your entire order!</p>
                <p id="countdown" style="font-weight: bold; margin-top: 10px;"></p>
            </div>

            <!-- Drink Sizes Reference -->
            <section class="drink-sizes fade-in">
                <h3>Our Drink Sizes</h3>
                <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_071625_Gallery.jpg" alt="Drink Sizes Reference">
                <p style="margin-top: 15px;">Small (350ml) | Medium (500ml) | Large (750ml)</p>
            </section>

            <!-- Menu Section -->
            <section class="menu-section">
                <div class="menu-category fade-in">
                    <h3>FRISS & 'KAK!</h3>
                    <div class="menu-items">
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Classic Crunch</span>
                                <span class="item-price">450/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070743_Gallery.jpg" alt="Classic Crunch" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">FRIES + 10 PCS MISHIKAKI + CHEF'S SIGNATURE SAUCE</p>
                            <span class="limited-edition">Limited Edition</span>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="classic-crunch">-</button>
                                    <span class="quantity" data-item="classic-crunch">0</span>
                                    <button class="quantity-btn plus" data-item="classic-crunch">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="classic-crunch" data-price="450">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Grand Sultan</span>
                                <span class="item-price">550/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070759_Gallery.jpg" alt="Grand Sultan" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">MEGA FRIES LOADED WITH 15 PCS MISHIKAKI + SPECIAL SAUCE</p>
                            <p class="item-desc">EXTRA MISHIKAKI @100/- PER SKEWER</p>
                            <span class="limited-edition">Limited Edition</span>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="grand-sultan">-</button>
                                    <span class="quantity" data-item="grand-sultan">0</span>
                                    <button class="quantity-btn plus" data-item="grand-sultan">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="grand-sultan" data-price="550">Add to Cart</button>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="menu-category fade-in">
                    <h3>FRESH JUICE</h3>
                    <div class="menu-items">
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Tangy Passion</span>
                                <span class="item-price" id="price-tangy-passion">250/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070846_Gallery.jpg" alt="Tangy Passion" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Bold Passion, Pure Tropical Energy</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="tangy-passion" data-size="small" data-price="250">Small: 250/-</button>
                                <button class="size-btn" data-item="tangy-passion" data-size="medium" data-price="350">Medium: 350/-</button>
                                <button class="size-btn" data-item="tangy-passion" data-size="large" data-price="450">Large: 450/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="tangy-passion">-</button>
                                    <span class="quantity" data-item="tangy-passion">0</span>
                                    <button class="quantity-btn plus" data-item="tangy-passion">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="tangy-passion" data-price="250">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Mango Rush</span>
                                <span class="item-price" id="price-mango-rush">250/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070846_Gallery.jpg" alt="Mango Rush" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Thick, Juicy, Naturally Sweet</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="mango-rush" data-size="small" data-price="250">Small: 250/-</button>
                                <button class="size-btn" data-item="mango-rush" data-size="medium" data-price="350">Medium: 350/-</button>
                                <button class="size-btn" data-item="mango-rush" data-size="large" data-price="450">Large: 450/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="mango-rush">-</button>
                                    <span class="quantity" data-item="mango-rush">0</span>
                                    <button class="quantity-btn plus" data-item="mango-rush">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="mango-rush" data-price="250">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Le' Pineapple De' Mint</span>
                                <span class="item-price" id="price-pineapple-mint">250/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070851_Gallery.jpg" alt="Le Pineapple De Mint" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Altuty Breeze, Pineapple Squeeze</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="pineapple-mint" data-size="small" data-price="250">Small: 250/-</button>
                                <button class="size-btn" data-item="pineapple-mint" data-size="medium" data-price="350">Medium: 350/-</button>
                                <button class="size-btn" data-item="pineapple-mint" data-size="large" data-price="450">Large: 450/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="pineapple-mint">-</button>
                                    <span class="quantity" data-item="pineapple-mint">0</span>
                                    <button class="quantity-btn plus" data-item="pineapple-mint">-</button>
                                </div>
                                <button class="btn add-to-cart" data-item="pineapple-mint" data-price="250">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Tropical Mix</span>
                                <span class="item-price" id="price-tropical-mix">250/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070856_Gallery.jpg" alt="Tropical Mix" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">All-in-one island infusion</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="tropical-mix" data-size="small" data-price="250">Small: 250/-</button>
                                <button class="size-btn" data-item="tropical-mix" data-size="medium" data-price="350">Medium: 350/-</button>
                                <button class="size-btn" data-item="tropical-mix" data-size="large" data-price="450">Large: 450/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="tropical-mix">-</button>
                                    <span class="quantity" data-item="tropical-mix">0</span>
                                    <button class="quantity-btn plus" data-item="tropical-mix">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="tropical-mix" data-price="250">Add to Cart</button>
                            </div>
                        </div>
                    </div>
                </div>
                
                <div class="menu-category fade-in">
                    <h3>MAGIC MOJITOS</h3>
                    <div class="menu-items">
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Blue Lagoon</span>
                                <span class="item-price" id="price-blue-lagoon">300/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070907_Gallery.jpg" alt="Blue Lagoon" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Tropical Citrus Wave, Blue Ocean</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="blue-lagoon" data-size="small" data-price="300">Small: 300/-</button>
                                <button class="size-btn" data-item="blue-lagoon" data-size="medium" data-price="400">Medium: 400/-</button>
                                <button class="size-btn" data-item="blue-lagoon" data-size="large" data-price="500">Large: 500/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="blue-lagoon">-</button>
                                    <span class="quantity" data-item="blue-lagoon">0</span>
                                    <button class="quantity-btn plus" data-item="blue-lagoon">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="blue-lagoon" data-price="300">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Red Flash</span>
                                <span class="item-price" id="price-red-flash">300/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070912_Gallery.jpg" alt="Red Flash" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Bold strawberry heat meets cool mint</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="red-flash" data-size="small" data-price="300">Small: 300/-</button>
                                <button class="size-btn" data-item="red-flash" data-size="medium" data-price="400">Medium: 400/-</button>
                                <button class="size-btn" data-item="red-flash" data-size="large" data-price="500">Large: 500/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="red-flash">-</button>
                                    <span class="quantity" data-item="red-flash">0</span>
                                    <button class="quantity-btn plus" data-item="red-flash">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="red-flash" data-price="300">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Berry Breeze</span>
                                <span class="item-price" id="price-berry-breeze">300/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070921_Gallery.jpg" alt="Berry Breeze" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Smooth berry chill, island style</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="berry-breeze" data-size="small" data-price="300">Small: 300/-</button>
                                <button class="size-btn" data-item="berry-breeze" data-size="medium" data-price="400">Medium: 400/-</button>
                                <button class="size-btn" data-item="berry-breeze" data-size="large" data-price="500">Large: 500/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="berry-breeze">-</button>
                                    <span class="quantity" data-item="berry-breeze">0</span>
                                    <button class="quantity-btn plus" data-item="berry-breeze">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="berry-breeze" data-price="300">Add to Cart</button>
                            </div>
                        </div>
                        
                        <div class="menu-item">
                            <div class="item-header">
                                <span class="item-name">Ginger Gold</span>
                                <span class="item-price" id="price-ginger-gold">300/-</span>
                            </div>
                            <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070926_Gallery.jpg" alt="Ginger Gold" style="width:100%; border-radius:10px; margin-bottom:15px;">
                            <p class="item-desc">Golden spice with honeyed flow</p>
                            <div class="size-options">
                                <button class="size-btn active" data-item="ginger-gold" data-size="small" data-price="300">Small: 300/-</button>
                                <button class="size-btn" data-item="ginger-gold" data-size="medium" data-price="400">Medium: 400/-</button>
                                <button class="size-btn" data-item="ginger-gold" data-size="large" data-price="500">Large: 极市500/-</button>
                            </div>
                            <div class="item-controls">
                                <div class="quantity-controls">
                                    <button class="quantity-btn minus" data-item="ginger-gold">-</button>
                                    <span class="quantity" data-item="ginger-gold">0</span>
                                    <button class="quantity-btn plus" data-item="ginger-gold">+</button>
                                </div>
                                <button class="btn add-to-cart" data-item="ginger-gold" data-price="300">Add to Cart</button>
                            </div>
                        </div>
                    </div>
                </div>
            </section>

            <!-- Checkout Form -->
            <section class="checkout-form" id="checkout-form">
                <h3>Complete Your Order</h3>
                <div class="form-group">
                    <label for="name">Full Name</label>
                    <input type="text" id="name" required>
                </div>
                <div class="form-group">
                    <label for="phone">Phone Number</label>
                    <input type="tel" id="phone" required>
                </div>
                <div class="form-group">
                    <label for="dressing">Dressing Description (Optional)</label>
                    <textarea id="dressing" rows="3"></textarea>
                </div>
                <div class="form-group">
                    <label for="location">Delivery Location</label>
                    <input type="text" id="delivery-location" readonly>
                    <small>If the location is not accurate, please describe your location below</small>
                </div>
                <div class="form-group">
                    <label for="location-details">Location Details (If needed)</label>
                    <textarea id="location-details" rows="2"></textarea>
                </div>
                
                <!-- Payment Information -->
                <div class="payment-info">
                    <h4>Payment Method</h4>
                    <p>We accept Lipa na M-Pesa</p>
                    <p><strong>Paybill:</strong> 542542</p>
                    <p><strong>Account Number:</strong> 786867</p>
                    <p>Please complete payment before placing your order</p>
                </div>
                
                <button class="checkout-btn" id="place-order">Place Order via WhatsApp</button>
            </section>
        </div>

        <!-- Floating Cart -->
        <div class="floating-cart cart-hidden" id="floating-cart">
            <div class="cart-header">
                <h3>Your Order</h3>
                <span id="cart-count">0 items</span>
            </div>
            <div class="cart-items" id="cart-items">
                <p style="text-align: center; padding: 20px;">Your cart is empty</p>
            </div>
            <div class="cart-total">
                <span>Total:</span>
                <span id="cart-total">0/-</span>
            </div>
            <button class="checkout-btn" id="checkout-btn">Proceed to Checkout</button>
        </div>

        <!-- Cart Toggle Button -->
        <div class="cart-toggle" id="cart-toggle">
            <i class="fas fa-shopping-cart"></i>
            <span class="cart-badge" id="cart-badge">0</span>
        </div>

        <!-- WhatsApp Chat -->
        <a href="https://wa.me/254115030726" class="whatsapp-chat" target="_blank">
            <i class="fab fa-whatsapp"></i>
        </a>
    </div>

    <!-- Footer -->
    <footer>
        <div class="container">
            <div class="footer-content">
                <div class="footer-about">
                    <h3>About Laansales101</h3>
                    <p>Laansales101 was born from a deep understanding of the challenges that vendors and event-goers face. What if there was a way to merge convenience with luxury, to transform an ordinary event into an extraordinary experience? That vision led to the creation of Laansales101—a cutting-edge platform designed to make ordering seamless, effortless, and uniquely personal for every event-goer.</p>
                </div>
                <div class="footer-contact">
                    <h3>Contact Us</h3>
                    <p><i class="fas fa-envelope"></i> emflavorsales@gmail.com</p>
                    <p><i class="fas fa-phone"></i> +254 115 030 726</p>
                    <p><i class="fab fa-whatsapp"></i> WhatsApp: +254 115 030 726</p>
                </div>
            </div>
            <div class="footer-logo">
                <img src="https://raw.githubusercontent.com/laansales999/Laan101emf/main/Images/Screenshot_20250831_070816_Gallery.jpg" alt="Laansale Logo">
            </div>
            <div class="footer-bottom">
                <p>&copy; 2025 Laansales101. All Rights Reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        // Initialize cart
        let cart = [];
        let userLocation = null;
        let lastScrollTop = 0;
        
        // DOM Elements
        const enableLocationBtn = document.getElementById('enableLocation');
        const locationStatus = document.getElementById('locationStatus');
        const checkoutBtn = document.getElementById('checkout-btn');
        const checkoutForm = document.getElementById('checkout-form');
        const placeOrderBtn = document.getElementById('place-order');
        const deliveryLocation = document.getElementById('delivery-location');
        const countdownEl = document.getElementById('countdown');
        const floatingCart = document.getElementById('floating-cart');
        const cartToggle = document.getElementById('cart-toggle');
        const cartBadge = document.getElementById('cart-badge');
        const mainHeader = document.getElementById('main-header');
        
        // Header scroll behavior
        window.addEventListener('scroll', function() {
            let scrollTop = window.pageYOffset || document.documentElement.scrollTop;
            
            if (scrollTop > lastScrollTop && scrollTop > 100) {
                // Scrolling down
                mainHeader.classList.add('header-hidden');
            } else {
                // Scrolling up
                mainHeader.classList.remove('header-hidden');
            }
            
            lastScrollTop = scrollTop;
        });
        
        // Cart toggle functionality
        let cartVisible = false;
        
        cartToggle.addEventListener('click', () => {
            cartVisible = !cartVisible;
            if (cartVisible) {
                floatingCart.classList.remove('cart-hidden');
            } else {
                floatingCart.classList.add('cart-hidden');
            }
        });
        
        // Enable location
        enableLocationBtn.addEventListener('click', () => {
            if (navigator.geolocation) {
                navigator.geolocation.getCurrentPosition(
                    position => {
                        userLocation = position;
                        const { latitude, longitude } = position.coords;
                        locationStatus.innerHTML = `Location enabled! Latitude: ${latitude.toFixed(6)}, Longitude: ${longitude.toFixed(6)}`;
                        locationStatus.style.color = '#10b981';
                        deliveryLocation.value = `${latitude.toFixed(6)}, ${longitude.toFixed(6)}`;
                        
                        // Try to get address from coordinates
                        getAddressFromCoords(latitude, longitude);
                    },
                    error => {
                        locationStatus.innerHTML = 'Unable to retrieve location. Please describe your location in the checkout form.';
                        locationStatus.style.color = '#ef4444';
                        deliveryLocation.value = 'Location not available. Please describe below.';
                    }
                );
            } else {
                locationStatus.innerHTML = 'Geolocation is not supported by this browser. Please describe your location in the checkout form.';
                locationStatus.style.color = '#ef4444';
                deliveryLocation.value = 'Geolocation not supported. Please describe below.';
            }
        });
        
        // Function to get address from coordinates
        function getAddressFromCoords(lat, lng) {
            // Using Nominatim (OpenStreetMap) for reverse geocoding
            fetch(`https://nominatim.openstreetmap.org/reverse?format=json&lat=${lat}&lon=${lng}`)
                .then(response => response.json())
                .then(data => {
                    if (data && data.display_name) {
                        deliveryLocation.value = data.display_name;
                    }
                })
                .catch(error => {
                    console.error('Error getting address:', error);
                });
        }
        
        // Size selection for drinks
        document.querySelectorAll('.size-btn').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const size = button.getAttribute('data-size');
                const price = button.getAttribute('data-price');
                
                // Remove active class from all buttons in this group
                button.parentNode.querySelectorAll('.size-btn').forEach(btn => {
                    btn.classList.remove('active');
                });
                
                // Add active class to clicked button
                button.classList.add('active');
                
                // Update price display
                document.getElementById(`price-${item}`).textContent = `${price}/-`;
                
                // Update add to cart button data-price
                const addButton = button.closest('.menu-item').querySelector('.add-to-cart');
                addButton.setAttribute('data-price', price);
            });
        });
        
        // Quantity controls
        document.querySelectorAll('.quantity-btn').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const quantityEl = document.querySelector(`.quantity[data-item="${item}"]`);
                let quantity = parseInt(quantityEl.textContent);
                
                if (button.classList.contains('plus')) {
                    quantity++;
                } else if (button.classList.contains('minus') && quantity > 0) {
                    quantity--;
                }
                
                quantityEl.textContent = quantity;
            });
        });
        
        // Add to cart
        document.querySelectorAll('.add-to-cart').forEach(button => {
            button.addEventListener('click', () => {
                const item = button.getAttribute('data-item');
                const price = parseInt(button.getAttribute('data-price'));
                const quantity = parseInt(document.querySelector(`.quantity[data-item="${item}"]`).textContent);
                
                if (quantity === 0) return;
                
                // Get selected size for drinks
                let size = null;
                const sizeBtn = button.closest('.menu-item').querySelector('.size-btn.active');
                if (sizeBtn) {
                    size = sizeBtn.getAttribute('data-size');
                }
                
                // Check if item already in cart
                const existingItemIndex = cart.findIndex(cartItem => 
                    cartItem.name === item && cartItem.size === size
                );
                
                if (existingItemIndex !== -1) {
                    cart[existingItemIndex].quantity += quantity;
                } else {
                    cart.push({
                        name: item,
                        price: price,
                        quantity: quantity,
                        size: size
                    });
                }
                
                updateCart();
                
                // Reset quantity
                document.querySelector(`.quantity[data-item="${item}"]`).textContent = '0';
                
                // Show cart
                floatingCart.classList.remove('cart-hidden');
                cartVisible = true;
            });
        });
        
        // Update cart
        function updateCart() {
            const cartItems = document.getElementById('cart-items');
            const cartCount = document.getElementById('cart-count');
            const cartTotal = document.getElementById('cart-total');
            
            // Clear cart items
            cartItems.innerHTML = '';
            
            if (cart.length === 0) {
                cartItems.innerHTML = '<p style="text-align: center; padding: 20px;">Your cart is empty</p>';
                cartCount.textContent = '0 items';
                cartTotal.textContent = '0/-';
                cartBadge.textContent = '0';
                return;
            }
            
            let total = 0;
            let itemCount = 0;
            
            cart.forEach((item, index) => {
                const itemTotal = item.price * item.quantity;
                total += itemTotal;
                itemCount += item.quantity;
                
                const cartItemEl = document.createElement('div');
                cartItemEl.className = 'cart-item';
                
                let sizeInfo = '';
                if (item.size) {
                    sizeInfo = ` (${item.size})`;
                }
                
                cartItemEl.innerHTML = `
                    <div class="cart-item-info">
                        <div>${formatItemName(item.name)}${sizeInfo}</div>
                        <div>${item.price}/- x ${item.quantity}</div>
                    </div>
                    <div class="cart-item-controls">
                        <span>${itemTotal}/-</span>
                        <button class="remove-btn" data-index="${index}">
                            <i class="fas fa-trash"></i>
                        </button>
                    </div>
                `;
                
                cartItems.appendChild(cartItemEl);
            });
            
            cartCount.textContent = `${itemCount} ${itemCount === 极市1 ? 'item' : 'items'}`;
            cartTotal.textContent = `${total}/-`;
            cartBadge.textContent = itemCount;
            
            // Add event listeners to remove buttons
            document.querySelectorAll('.remove-btn').forEach(button => {
                button.addEventListener('click', () => {
                    const index = parseInt(button.getAttribute('data-index'));
                    cart.splice(index, 1);
                    updateCart();
                });
            });
        }
        
        // Format item name for display
        function formatItemName(name) {
            return name.split('-')
                .map(word => word.charAt(0).toUpperCase() + word.slice(1))
                .join(' ');
        }
        
        // Checkout button
        checkoutBtn.addEventListener('click', () => {
            if (cart.length === 0) {
                alert('Your cart is empty. Please add items before checkout.');
                return;
            }
            
            checkoutForm.style.display = 'block';
            checkoutForm.scrollIntoView({ behavior: 'smooth' });
        });
        
        // Place order
        placeOrderBtn.addEventListener('click', () => {
            const name = document.getElementById('name').value;
            const phone = document.getElementById('phone').value;
            
            if (!name || !phone) {
                alert('Please fill in all required fields.');
                return;
            }
            
            // Create order summary
            let orderSummary = `*NEW ORDER FROM EXQUISITE MADIWA FLAVORS WEBSITE*\n\n`;
            orderSummary += `*Customer Name:* ${name}\n`;
            orderSummary += `*Phone:* ${phone}\n`;
            
            // Add location information
            const locationDetails = document.getElementById('location-details').value;
            if (deliveryLocation.value && deliveryLocation.value !== 'Location not available. Please describe below.') {
                orderSummary += `*Location:* ${deliveryLocation.value}\n`;
            }
            if (locationDetails) {
                orderSummary += `*Location Details:* ${locationDetails}\n`;
            }
            
            orderSummary += `\n*Order Details:*\n`;
            
            cart.forEach(item => {
                let sizeInfo = '';
                if (item.size) {
                    sizeInfo = ` (${item.size})`;
                }
                orderSummary += `- ${formatItemName(item.name)}${sizeInfo} x ${item.quantity} = ${item.price * item.quantity}/-\n`;
            });
            
            orderSummary += `\n*Total: ${cart.reduce((total, item) => total + (item.price * item.quantity), 极市0)}/-*\n\n`;
            
            const dressing = document.getElementById('dressing').value;
            if (dressing) {
                orderSummary += `*Dressing Instructions:* ${dressing}\n`;
            }
            
            orderSummary += `\n*Payment Method:* Lipa na M-Pesa\n`;
            orderSummary += `*Paybill:* 542542\n`;
            orderSummary += `*Account Number:* 786867\n`;
            
            // Encode for WhatsApp URL
            const encodedMessage = encodeURIComponent(orderSummary);
            const whatsappURL = `https://wa.me/254115030726?text=${encodedMessage}`;
            
            // Open WhatsApp
            window.open(whatsappURL, '_blank');
            
            // Reset极市 cart and form
            cart = [];
            updateCart();
            checkoutForm.style.display = 'none';
            document.getElementById('name').value = '';
            document.getElementById('phone').value = '';
            document.getElementById('dressing').value = '';
            document.getElementById极市('location-details').value = '';
            
            alert('Your order has been placed! You will be redirected to WhatsApp to confirm.');
        });
        
        // Countdown timer for special offer
        function updateCountdown() {
            const now = new Date();
            const minutes极市 = now.getMinutes();
            const seconds = now.getSeconds();
            
            if (minutes < 20) {
                const timeLeft = 20 - minutes;
                const secsLeft = 60 - seconds;
                countdownEl.textContent = `Offer ends in: ${timeLeft} min ${secsLeft} sec`;
            } else {
                const nextHour = new Date(now);
                nextHour.setHours(nextHour.getHours() + 1);
                nextHour.setMinutes(0);
                nextHour.setSeconds(0);
                
                const diff = nextHour - now;
                const minsLeft = Math.floor(diff / 60000);
                const secsLeft = Math.floor((diff % 60000) / 1000);
                
                countdownEl.textContent = `Next offer in: ${minsLeft} min ${secsLeft} sec`;
            }
        }
        
        setInterval(updateCountdown, 1000);
        updateCountdown();
        
        // Add fade-in animation to elements when they come into view
        const fadeElements = document.querySelectorAll('.fade-in');
        
        const fadeInObserver = new IntersectionObserver((entries) => {
            entries.forEach(entry => {
                if (entry.isIntersecting) {
                    entry.target.style.animation = 'fadeIn 1s ease forwards';
                    fadeInObserver.unobserve(entry.target);
                }
            });
        }, { threshold: 0.1 });
        
        fadeElements.forEach(element => {
            fadeInObserver.observe(element);
        });
    </script>
</body>
</html>
