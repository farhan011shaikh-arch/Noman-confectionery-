<think>
First, the user said "Make totally complete please". They want the entire website code in one complete HTML file, including CSS and JS embedded.

</think>```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Numan Confectionery - Fresh Bakery Delights</title>
    <link rel="icon" href="https://via.placeholder.com/32x32?text=🍰" type="image/x-icon">
    <style>
        /* Reset and Base Styles */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }
        body {
            font-family: 'Arial', sans-serif;
            line-height: 1.6;
            color: #333;
            background-color: #f9f4f0;
        }
        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 20px;
        }
        h1, h2, h3, h4 {
            color: #8b4513;
        }
        .btn {
            display: inline-block;
            background-color: #d2691e;
            color: white;
            padding: 10px 20px;
            text-decoration: none;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        .btn:hover {
            background-color: #a0522d;
        }
        .small-btn {
            padding: 5px 10px;
            font-size: 0.9em;
        }

        /* Header */
        header {
            background-color: #fff;
            box-shadow: 0 2px 5px rgba(0,0,0,0.1);
            position: sticky;
            top: 0;
            z-index: 100;
        }
        header .container {
            display: flex;
            justify-content: space-between;
            align-items: center;
            padding: 20px;
        }
        nav a {
            margin: 0 15px;
            text-decoration: none;
            color: #333;
            font-weight: bold;
        }
        nav a:hover {
            color: #d2691e;
        }
        #cart-icon {
            font-size: 1.1em;
        }

        /* Hero */
        #hero {
            background-image: url('https://images.unsplash.com/photo-1578985545062-69928b1d9587?w=1200&h=400&fit=crop');
            background-size: cover;
            background-position: center;
            color: white;
            text-align: center;
            padding: 100px 20px;
        }
        #hero h2 {
            font-size: 2.5em;
            margin-bottom: 20px;
        }
        #hero p {
            font-size: 1.2em;
            margin-bottom: 30px;
        }

        /* Product Sections */
        .product-section {
            padding: 50px 0;
            background-color: #fff;
        }
        .products {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
            justify-content: center;
        }
        .product {
            background-color: #f9f4f0;
            border-radius: 10px;
            padding: 20px;
            text-align: center;
            width: 300px;
            box-shadow: 0 2px 10px rgba(0,0,0,0.1);
        }
        .product img {
            width: 100%;
            height: 200px;
            object-fit: cover;
            border-radius: 5px;
        }
        .product h3, .product h4 {
            margin: 15px 0;
        }
        .price {
            font-size: 1.2em;
            color: #d2691e;
            font-weight: bold;
        }
        .add-btn, .whatsapp-btn {
            margin-top: 10px;
        }
        .upload-btn {
            margin: 10px 0;
        }
        #preview {
            border-radius: 5px;
        }

        /* Special Orders */
        .subcategories {
            display: flex;
            flex-wrap: wrap;
            gap: 20px;
        }
        .subcategory {
            flex: 1;
            min-width: 300px;
        }

        /* Other Sections */
        #why-choose-us, #testimonials, #buy-now, footer {
            padding: 50px 0;
            text-align: center;
            background-color: #f9f4f0;
        }
        #why-choose-us ul {
            list-style: none;
            padding: 0;
        }
        #why-choose-us li {
            margin: 10px 0;
        }
        .testimonial {
            margin: 20px 0;
            font-style: italic;
        }

        /* Scroll to Top */
        #scroll-to-top {
            position: fixed;
            bottom: 20px;
            right: 20px;
            display: none;
        }

        /* Responsive */
        @media (max-width: 768px) {
            header .container {
                flex-direction: column;
                text-align: center;
            }
            nav {
                margin: 10px 0;
            }
            .products {
                flex-direction: column;
                align-items: center;
            }
            .product {
                width: 100%;
                max-width: 300px;
            }
        }
    </style>
</head>
<body>
    <header>
        <div class="container">
            <h1>Numan Confectionery</h1>
            <nav>
                <a href="#cakes">Cakes</a>
                <a href="#pastries">Pastries</a>
                <a href="#biscuits">Biscuits</a>
                <a href="#sweets">Sweets</a>
                <a href="#bakery-items">Bakery Items</a>
                <a href="#custom-birthday">Custom Birthday Cakes</a>
                <a href="#special-orders">Special Orders</a>
                <a href="#why-choose-us">Why Choose Us?</a>
                <a href="#testimonials">Testimonials</a>
                <a href="#contact">Contact</a>
            </nav>
            <div id="cart-icon">Cart: <span id="cart-count">0</span> items <button id="clear-cart" class="btn small-btn">Clear</button></div>
        </div>
    </header>

    <section id="hero">
        <div class="container">
            <h2>Fresh, Original Bakery Treats</h2>
            <p>Indulge in our handcrafted cakes, pastries, biscuits, sweets, and more. Made with love and the finest ingredients.</p>
            <a href="#cakes" class="btn">Explore Products</a>
        </div>
    </section>

    <section id="cakes" class="product-section">
        <div class="container">
            <h2>Cakes</h2>
            <div class="products">
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?w=400&h=300&fit=crop" alt="Chocolate Cake">
                    <h3>Chocolate Delight Cake</h3>
                    <p class="price">₹500</p>
                    <button class="add-btn" data-product="Chocolate Delight Cake" data-price="500">Add to Cart</button>
                </div>
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1621303837174-89787a7d4729?w=400&h=300&fit=crop" alt="Vanilla Cake">
                    <h3>Vanilla Dream Cake</h3>
                    <p class="price">₹450</p>
                    <button class="add-btn" data-product="Vanilla Dream Cake" data-price="450">Add to Cart</button>
                </div>
            </div>
        </div>
    </section>

    <section id="pastries" class="product-section">
        <div class="container">
            <h2>Pastries</h2>
            <div class="products">
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1555507036-ab1f4038808a?w=400&h=300&fit=crop" alt="Croissant">
                    <h3>Butter Croissant</h3>
                    <p class="price">₹100</p>
                    <button class="add-btn" data-product="Butter Croissant" data-price="100">Add to Cart</button>
                </div>
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1507003211169-0a1dd7228f2d?w=400&h=300&fit=crop" alt="Danish Pastry">
                    <h3>Fruit Danish</h3>
                    <p class="price">₹150</p>
                    <button class="add-btn" data-product="Fruit Danish" data-price="150">Add to Cart</button>
                </div>
            </div>
        </div>
    </section>

    <section id="biscuits" class="product-section">
        <div class="container">
            <h2>Biscuits</h2>
            <div class="products">
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1558961363-fa8fdf82db35?w=400&h=300&fit=crop" alt="Chocolate Chip Cookies">
                    <h3>Chocolate Chip Cookies</h3>
                    <p class="price">₹250</p>
                    <button class="add-btn" data-product="Chocolate Chip Cookies" data-price="250">Add to Cart</button>
                </div>
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1499636136210-6f4ee915583e?w=400&h=300&fit=crop" alt="Shortbread Biscuits">
                    <h3>Shortbread Biscuits</h3>
                    <p class="price">₹200</p>
                    <button class="add-btn" data-product="Shortbread Biscuits" data-price="200">Add to Cart</button>
                </div>
            </div>
        </div>
    </section>

    <section id="sweets" class="product-section">
        <div class="container">
            <h2>Sweets</h2>
            <div class="products">
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1606312619070-d48b4c652a52?w=400&h=300&fit=crop" alt="Ras Malai">
                    <h3>Ras Malai</h3>
                    <p class="price">₹300</p>
                    <button class="add-btn" data-product="Ras Malai" data-price="300">Add to Cart</button>
                </div>
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1551024506-0bccd828d307?w=400&h=300&fit=crop" alt="Gulab Jamun">
                    <h3>Gulab Jamun</h3>
                    <p class="price">₹350</p>
                    <button class="add-btn" data-product="Gulab Jamun" data-price="350">Add to Cart</button>
                </div>
            </div>
        </div>
    </section>

    <section id="bakery-items" class="product-section">
        <div class="container">
            <h2>Bakery Items</h2>
            <div class="products">
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1509440159596-0249088772ff?w=400&h=300&fit=crop" alt="Bread Loaf">
                    <h3>Artisan Bread Loaf</h3>
                    <p class="price">₹300</p>
                    <button class="add-btn" data-product="Artisan Bread Loaf" data-price="300">Add to Cart</button>
                </div>
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1586444248902-2f64eddc13df?w=400&h=300&fit=crop" alt="Muffins">
                    <h3>Blueberry Muffins</h3>
                    <p class="price">₹180</p>
                    <button class="add-btn" data-product="Blueberry Muffins" data-price="180">Add to Cart</button>
                </div>
            </div>
        </div>
    </section>

    <section id="custom-birthday" class="product-section">
        <div class="container">
            <h2>Custom Birthday Cakes</h2>
            <div class="products">
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1535254973040-607b474cb50d?w=400&h=300&fit=crop" alt="Custom Cake">
                    <h3>Personalized Theme Cake</h3>
                    <p class="price">₹800</p>
                    <button class="add-btn" data-product="Personalized Theme Cake" data-price="800">Add to Cart</button>
                </div>
                <div class="product">
                    <img src="https://images.unsplash.com/photo-1606312619070-d48b4c652a52?w=400&h=300&fit=crop" alt="Fondant Cake">
                    <h3>Fondant Birthday Cake</h3>
                    <p class="price">₹1000</p>
                    <button class="add-btn" data-product="Fondant Birthday Cake" data-price="1000">Add to Cart</button>
                </div>
            </div>
        </div>
    </section>

    <section id="special-orders" class="product-section">
        <div class="container">
            <h2>Special Orders</h2>
            <div class="subcategories">
                <div class="subcategory">
                    <h3>Birthday Cakes</h3>
                    <div class="products">
                        <div class="product">
                            <img src="https://images.unsplash.com/photo-1578985545062-69928b1d9587?w=400&h=300&fit=crop" alt="Birthday Cake">
                            <h4>Chocolate Birthday Cake</h4>
                            <p class="price">₹600</p>
                            <a href="https://wa.me/918369701874?text=Hi%20Numan%20Confectionery,%20I%20want%20to%20order%20a%20Chocolate%20Birthday%20Cake" class="btn whatsapp-btn">Order on WhatsApp</a>
                        </div>
                    </div>
                </div>
                <div class="subcategory">
                    <h3>Anniversary Cakes</h3>
                    <div class="products">
                        <div class="product">
                            <img src="https://images.unsplash.com/photo-1621303837174-89787a7d4729?w=400&h=300&fit=crop" alt="Anniversary Cake">
                            <h4>Red Velvet Anniversary Cake</h4>
                            <p class="price">₹700</p>
                            <a href="https://wa.me/918369701874?text=Hi%20Numan%20Confectionery,%20I%20want%20to%20order%20a%20Red%20Velvet%20Anniversary%20Cake" class="btn whatsapp-btn">Order on WhatsApp</a>
                        </div>
                    </div>
                </div>
                <div class="subcategory">
                    <h3>Custom Design Cakes</h3>
                    <div class="products">
                        <div class="product">
                            <img src="https://images.unsplash.com/photo-1535254973040-607b474cb50d?w=400&h=300&fit=crop" alt="Custom Cake">
                            <h4>Custom Design Cake</h4>
                            <p class="price">₹1200</p>
                            <input type="file" id="custom-image" accept="image/*" class="upload-btn">
                            <img id="preview" src="" alt="Preview" style="display:none; width:100px; height:100px; margin:10px;">
                            <a href="https://wa.me/918369701874?text=Hi%20Numan%20Confectionery,%20I%20want%20to%20order%20a%20Custom%20Design%20Cake" class="btn whatsapp-btn">Order on WhatsApp</a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="why-choose-us">
        <div class="container">
            <h2>Why Choose Us?</h2>
            <ul>
                <li><strong>Fresh Ingredients:</strong> We use only the freshest, high-quality ingredients in every product.</li>
                <li><strong>Hygienic Kitchen:</strong> Our kitchen follows strict hygiene standards for safe and clean baking.</li>
                <li><strong>Affordable Price:</strong> Enjoy premium bakery items at prices that fit your budget.</li>
            </ul>
        </div>
    </section>

    <section id="testimonials">
        <div class="container">
            <h2>What Our Customers Say</h2>
            <div class="testimonial">
                <p>"Amazing cakes! Fresh and delicious." - Priya S.</p>
            </div>
            <div class="testimonial">
                <p>"Best pastries in town. Highly recommend!" - Rahul M.</p>
            </div>
        </div>
    </section>

    <section id="buy-now">
        <div class="container">
            <h2>Ready to Order?</h2>
            <button id="buy-btn" class="btn">Buy Now</button>
        </div>
    </section>

    <footer id="contact">
        <div class="container">
            <p>Contact Us: Call +91 83697 01874 | Email: info@numanconfectionery.com</p>
            <p>&copy; 2023 Numan Confectionery. All rights reserved.</p>
        </div>
    </footer>

    <button id="scroll-to-top" class="btn">↑ Top</button>

    <script>
        // Initialize cart from localStorage or empty array
        let cart = JSON.parse(localStorage.getItem('cart')) || [];
        updateCartCount();

        // Function to update cart count in header
        function updateCartCount() {
            const cartCount = document.getElementById('cart-count');
            cartCount.text
