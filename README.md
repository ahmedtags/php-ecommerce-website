# PHP E-Commerce Website

<p align="center">
  <img src="https://img.shields.io/badge/Language-PHP%20%26%20MySQL-777BB4?style=for-the-badge&logo=php&logoColor=white" alt="Language" />
  <img src="https://img.shields.io/badge/Course-Web%20Dev-24292e?style=for-the-badge" alt="Course" />
  <a href="https://github.com/ahmedtags">
    <img src="https://img.shields.io/badge/Profile-ahmedtags-D9A34A?style=for-the-badge&logo=github&logoColor=white" alt="Profile" />
  </a>
  <a href="https://blxman-37fy.vercel.app/">
    <img src="https://img.shields.io/badge/Portfolio-blxman--37fy-0A66C2?style=for-the-badge&logo=googlechrome&logoColor=white" alt="Portfolio" />
  </a>
</p>

---

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

---

## 📸 Database Schema

Here is the database structure defined in `DATABASE FILE/ecom_store.sql` to support the e-commerce shop system:

| Table Name | Description | Key Fields |
|------------|-------------|------------|
| `admins` | Store admin credentials and profiles | `admin_id`, `admin_email`, `admin_pass` |
| `customers` | Customer registration information | `customer_id`, `customer_email`, `customer_pass` |
| `products` | Product listings, details, pricing | `product_id`, `product_title`, `product_price` |
| `product_categories` | Product sub-categories | `p_cat_id`, `p_cat_title` |
| `categories` | Main categories (Men, Women, Kids) | `cat_id`, `cat_title` |
| `cart` | Temporary items in user shopping carts | `p_id`, `ip_add`, `qty` |
| `customer_orders` | Orders placed by customers | `order_id`, `customer_id`, `due_amount` |
| `payments` | Customer order payments tracking | `payment_id`, `invoice_no`, `amount` |
| `coupons` | Promo codes and discounts | `coupon_id`, `coupon_code`, `coupon_price` |
| `wishlist` | Customer saved favorite items | `wishlist_id`, `customer_id`, `product_id` |
| `store` | Physical store locations details | `store_id`, `store_title`, `store_desc` |
| `terms` | Store terms & conditions | `term_id`, `term_title`, `term_desc` |
