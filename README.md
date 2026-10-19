# Alpha Moussa Sow — Portfolio

Responsive French/English portfolio built with PHP, MySQL, HTML, CSS, and JavaScript. The site includes a dynamic projects page, an admin area for project and technology management, and a contact page with email and WhatsApp options.

## Requirements

- PHP 8.1+ with PDO MySQL, fileinfo, mbstring, and sessions
- MySQL 5.7+ or MariaDB 10.3+
- Apache/XAMPP or compatible PHP hosting

## Local setup

1. Put the project in your PHP web root and install dependencies with Composer (`composer install`).
2. Create a MySQL database and import `database/schema.sql`.
3. Open the site through the local web server. The setup wizard creates the private `.env` configuration and admin account.
4. Sign in at `/admin/login.php` to manage projects and technologies.

Never commit `.env`, uploaded media, local setup markers, or private project notes. `.env.example` contains placeholders only. Keep the upload-directory `.htaccess` files in place to prevent uploaded scripts from executing.

## Main routes

- `/` — portfolio home page
- `/about.html`, `/skills.html`, `/experience.html`, `/contact.html` — portfolio sections
- `/projects/index.php` — published projects and category filters
- `/admin/login.php` — admin sign-in
- `/api/projects.php` and `/api/technologies.php` — public JSON endpoints

The site uses a fixed dark theme, reduced-motion preferences, and a French/English language toggle.