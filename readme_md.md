# Web Development - Activity-Based Learning (ABL) Assignment

**Institution:** Dr. RVR NRI Institute of Technology  
**Department:** School of Computer Studies  
**Course:** Web Development  

---

## Student Details

* **Name:** Y. Raghu Ram  
* **Roll Number:** 26000071  
* **Branch:** Computer Science and Engineering (CSE)  
* **Section:** CSE - 1  

---

## Selected Case Studies

1. **Case Study 1:** Personal Portfolio Website
2. **Case Study 6:** Online Shopping Website (ShopMart)
3. **Case Study 28:** User Registration and Login Interface

---

## Case Study 1: Personal Portfolio Website

### Description
A personal website displaying a developer profile, technical skills, project showcase, and contact information built using semantic HTML5 and CSS3 styling with responsive design elements.

### Source Code (`case1.html`)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Personal Portfolio</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: Arial, sans-serif; }
        body { line-height: 1.6; color: #db2929; background-color: #f9f9f9; }
        header { background: #2e6fb1; color: #fff; padding: 1rem 2rem; display: flex; justify-content: space-between; align-items: center; position: sticky; top: 0; }
        nav a { color: #fff; text-decoration: none; margin-left: 20px; transition: color 0.3s; }
        nav a:hover { color: #1abc9c; }
        .hero { text-align: center; padding: 4rem 2rem; background: #34495e; color: #fff; }
        .container { max-width: 1000px; margin: 2rem auto; padding: 0 20px; }
        section { background: #fff; margin-bottom: 2rem; padding: 2rem; border-radius: 8px; box-shadow: 0 2px 5px rgba(0,0,0,0.1); }
        h2 { margin-bottom: 1rem; color: #2c3e50; border-bottom: 2px solid #1abc9c; display: inline-block; padding-bottom: 5px; }
        .skills-list, .project-grid { display: flex; gap: 15px; flex-wrap: wrap; margin-top: 1rem; }
        .skill-badge { background: #1abc9c; color: white; padding: 8px 15px; border-radius: 20px; font-size: 0.9rem; }
        .project-card { border: 1px solid #ddd; padding: 15px; border-radius: 5px; flex: 1; min-width: 250px; background: #fafafa; }
        footer { text-align: center; padding: 1.5rem; background: #2c3e50; color: white; margin-top: 2rem; }
    </style>
</head>
<body>
    <header>
        <h1>raghu ram.y</h1>
        <nav>
            <a href="#about">About</a>
            <a href="#skills">Skills</a>
            <a href="#projects">Projects</a>
            <a href="#contact">Contact</a>
        </nav>
    </header>

    <section class="hero" id="about">
        <h2>Web Developer & Designer</h2>
        <p>Creating responsive layouts, modern user interfaces, and engaging digital experiences.</p>
    </section>

    <div class="container">
        <section id="skills">
            <h2>Technical Skills</h2>
            <div class="skills-list">
                <span class="skill-badge">HTML5 / CSS3</span>
                <span class="skill-badge">JavaScript</span>
                <span class="skill-badge">Responsive Design</span>
                <span class="skill-badge">Git & GitHub</span>
            </div>
        </section>

        <section id="projects">
            <h2>Projects</h2>
            <div class="project-grid">
                <div class="project-card">
                    <h3>E-Commerce Dashboard</h3>
                    <p>A fully responsive admin dashboard layout built using CSS Grid and Flexbox.</p>
                </div>
                <div class="project-card">
                    <h3>Task Manager App</h3>
                    <p>An interactive task tracking application featuring dynamic DOM manipulation.</p>
                </div>
            </div>
        </section>

        <section id="contact">
            <h2>Contact Information</h2>
            <p>Email: john.doe@example.com</p>
            <p>Phone: +1 (555) 123-4567</p>
        </section>
    </div>

    <footer>
        <p>&copy; 2026 John Doe. All rights reserved.</p>
    </footer>
</body>
</html>
```

### Output Screenshot
![Personal Portfolio Website](Screenshot%202026-10-24%20134739.png)

---

## Case Study 6: Online Shopping Website

### Description
An e-commerce store interface featuring product cards with price tags, discount badges, customer star ratings, promotional banners, and responsive layout grids.

### Source Code (`case2.html`)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Online Shopping Store</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: Arial, sans-serif; }
        body { background-color: #f4f4f4; }
        nav { background: #232f3e; color: white; padding: 1rem 2rem; display: flex; justify-content: space-between; align-items: center; }
        .banner { background: #febd69; color: #111; text-align: center; padding: 2rem; font-size: 1.5rem; font-weight: bold; }
        .container { max-width: 1200px; margin: 2rem auto; padding: 0 20px; }
        .product-grid { display: grid; grid-template-columns: repeat(auto-fit, minmax(250px, 1fr)); gap: 20px; }
        .product-card { background: white; border: 1px solid #ddd; border-radius: 4px; padding: 15px; position: relative; text-align: center; }
        .discount-badge { position: absolute; top: 10px; left: 10px; background: #cc0c39; color: white; padding: 4px 8px; font-size: 0.8rem; border-radius: 3px; }
        .product-img { width: 100%; height: 180px; background: #e2e2e2; display: flex; align-items: center; justify-content: center; margin-bottom: 15px; color: #777; }
        .price { font-size: 1.2rem; color: #B12704; font-weight: bold; margin: 10px 0; }
        .rating { color: #ffa41c; margin-bottom: 10px; }
        .buy-btn { background: #ffd814; border: 1px solid #fcd200; width: 100%; padding: 10px; border-radius: 20px; cursor: pointer; font-weight: bold; transition: background 0.2s; }
        .buy-btn:hover { background: #f7ca00; }
    </style>
</head>
<body>
    <nav>
        <h1>ShopMart</h1>
        <div>Cart (0)</div>
    </nav>

    <div class="banner">Special Seasonal Discount - Up to 50% Off!</div>

    <div class="container">
        <div class="product-grid">
            <div class="product-card">
                <span class="discount-badge">20% OFF</span>
                <div class="product-img">Product Image</div>
                <h3>Wireless Headphones</h3>
                <div class="rating">★★★★☆ (120)</div>
                <div class="price">$79.99</div>
                <button class="buy-btn">Add to Cart</button>
            </div>
            <div class="product-card">
                <span class="discount-badge">15% OFF</span>
                <div class="product-img">Product Image</div>
                <h3>Smart Watch</h3>
                <div class="rating">★★★★★ (85)</div>
                <div class="price">$129.99</div>
                <button class="buy-btn">Add to Cart</button>
            </div>
            <div class="product-card">
                <span class="discount-badge">30% OFF</span>
                <div class="product-img">Product Image</div>
                <h3>Running Shoes</h3>
                <div class="rating">★★★★☆ (230)</div>
                <div class="price">$49.99</div>
                <button class="buy-btn">Add to Cart</button>
            </div>
        </div>
    </div>
</body>
</html>
```

### Output Screenshot
![Online Shopping Website](Screenshot%202026-10-24%20134850.png)

---

## Case Study 28: User Registration and Login Interface

### Description
A clean, responsive authentication card interface with input validation fields, labels, submit buttons, and dynamic state styling.

### Source Code (`case3.html`)
```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Registration and Login</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; font-family: Arial, sans-serif; }
        body { background: #eef2f3; display: flex; justify-content: center; align-items: center; height: 100vh; }
        .auth-container { background: white; padding: 2rem; border-radius: 8px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); width: 100%; max-width: 400px; }
        h2 { margin-bottom: 1.5rem; color: #333; text-align: center; }
        .form-group { margin-bottom: 1rem; }
        label { display: block; margin-bottom: 5px; font-weight: bold; color: #555; }
        input { width: 100%; padding: 10px; border: 1px solid #ccc; border-radius: 4px; font-size: 1rem; }
        input:focus { border-color: #007bff; outline: none; box-shadow: 0 0 5px rgba(0, 123, 255, 0.3); }
        .submit-btn { width: 100%; padding: 10px; background: #007bff; border: none; color: white; font-size: 1rem; border-radius: 4px; cursor: pointer; margin-top: 10px; }
        .submit-btn:hover { background: #0056b3; }
        .toggle-text { text-align: center; margin-top: 15px; font-size: 0.9rem; }
        .toggle-text a { color: #007bff; text-decoration: none; }
        .toggle-text a:hover { text-decoration: underline; }
    </style>
</head>
<body>
    <div class="auth-container">
        <h2>Create Account</h2>
        <form action="#" method="POST">
            <div class="form-group">
                <label for="fullname">Full Name</label>
                <input type="text" id="fullname" name="fullname" required placeholder="Enter your full name">
            </div>
            <div class="form-group">
                <label for="email">Email Address</label>
                <input type="email" id="email" name="email" required placeholder="Enter your email">
            </div>
            <div class="form-group">
                <label for="password">Password</label>
                <input type="password" id="password" name="password" required minlength="6" placeholder="At least 6 characters">
            </div>
            <button type="submit" class="submit-btn">Register</button>
        </form>
        <div class="toggle-text">
            Already have an account? <a href="#">Login here</a>
        </div>
    </div>
</body>
</html>
```

### Output Screenshot
![User Registration and Login Interface](Screenshot%202026-10-24%20134956.png)