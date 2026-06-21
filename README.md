# PHP E-Commerce Website

A fully functional e-commerce shopping cart web application built with **PHP** and **MySQL**. Features include product listings, customer authentication, a shopping cart, checkout, admin panel, and PayPal payment integration.

---

## Features

- **Product Catalog** — Browse products by category with detail pages
- **Shopping Cart** — Add/remove items, update quantities, view cart total
- **Customer Authentication** — Register, login, logout, and forgot password flows
- **Checkout & Orders** — Order placement and order tracking for customers
- **Admin Panel** — Manage products, orders, and customer accounts
- **PayPal Integration** — PayPal checkout for secure payments
- **Responsive UI** — Clean, mobile-friendly design using CSS and Font Awesome

---

## Project Structure

```
ecommerce-website-php/
├── index.php            # Home page — featured products
├── shop.php             # Full product catalog
├── details.php          # Individual product page
├── cart.php             # Shopping cart
├── checkout.php         # Checkout flow
├── customer_register.php # Customer registration
├── customer/            # Customer profile pages
├── admin_area/          # Admin panel (manage products, orders)
├── functions/           # Database query helpers
├── includes/            # Header, footer, and common includes
├── DATABASE FILE/       # SQL database schema dump
├── styles/              # CSS stylesheets
├── js/                  # JavaScript files
└── images/              # Product and site images
```

---

## Tools & Tech Stack

- **Backend:** PHP (native, no framework)
- **Database:** MySQL
- **Frontend:** HTML, CSS, JavaScript, Font Awesome
- **Payments:** PayPal integration

---

## How to Run Locally

1. Install a local PHP + MySQL server (e.g., **XAMPP**, **WAMP**, or **Laragon**).
2. Clone or copy the project into your server's `htdocs` (XAMPP) or `www` (WAMP) folder.
3. Import the SQL file from `DATABASE FILE/` into MySQL using phpMyAdmin or the CLI:
   ```bash
   mysql -u root -p your_db_name < "DATABASE FILE/database.sql"
   ```
4. Update database credentials in the connection configuration file (usually `functions/` or `includes/`).
5. Navigate to `http://localhost/ecommerce-website-php/` in your browser.
