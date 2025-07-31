# Laravel + Filament Boilerplate

<p align="center">
<a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="300" alt="Laravel Logo"></a>
<a href="https://filamentphp.com" target="_blank"><img src="https://filamentphp.com/images/social.png" width="300" alt="Filament Logo"></a>
</p>

<p align="center">
<img src="https://img.shields.io/badge/Laravel-12-red?style=flat-square&logo=laravel" alt="Laravel 12">
<img src="https://img.shields.io/badge/Filament-3.3-blue?style=flat-square&logo=filament" alt="Filament v3.3">
<img src="https://img.shields.io/badge/PHP-8.2-purple?style=flat-square&logo=php" alt="PHP 8.2">
<img src="https://img.shields.io/github/license/apriansyahrs/filament?style=flat-square" alt="License">
</p>

## 🚀 About This Boilerplate

Boilerplate siap pakai untuk project Laravel dengan Filament Admin Panel yang sudah dikonfigurasi. Tidak perlu repot-repot setup dari nol, tinggal clone dan jalankan satu command untuk memulai development!

### ✨ What's Included

- **Laravel 12** - Framework PHP modern dan powerful
- **Filament v3.3** - Admin panel yang elegant dan feature-rich
- **Pre-configured setup** - Semua konfigurasi sudah siap pakai
- **One-command installation** - Setup Filament dengan satu command
- **Clean structure** - Struktur project yang rapi dan terorganisir

### 🛠️ Tech Stack

- **Backend**: Laravel 12
- **Admin Panel**: Filament v3.3
- **Database**: SQLite (default) / MySQL / PostgreSQL
- **Frontend**: Blade Templates + Tailwind CSS (via Filament)
- **Build Tool**: Vite

## 🏃‍♂️ Quick Start

### Prerequisites

- PHP 8.2 atau lebih tinggi
- Composer
- Node.js & NPM
- Git

### Installation

1. **Clone repository ini:**
   ```bash
   git clone https://github.com/apriansyahrs/filament.git
   cd filament
   ```

2. **Setup Filament (One Command Setup):**
   ```bash
   composer run install-filament
   ```
   
   Command ini akan:
   - Copy `.env.example` ke `.env` (jika belum ada)
   - Install semua Composer dependencies
   - Install Filament package
   - Setup Filament panels
   - Jalankan migrasi database
   - Buat user admin untuk Filament

3. **Install NPM dependencies & Build assets:**
   ```bash
   npm install
   npm run build
   # atau untuk development
   npm run dev
   ```

4. **Start development server:**
   ```bash
   php artisan serve
   ```

5. **Access admin panel:**
   - URL: `http://localhost:8000/admin`
   - Login dengan kredensial yang dibuat saat step 3

## 📝 Available Commands

### Development
```bash
# Start all development services (server, queue, logs, vite)
composer run dev

# Run tests
composer run test

# Setup Filament (if needed)
composer run install-filament
```

### Artisan Commands
```bash
# Create Filament resource
php artisan make:filament-resource Post

# Create Filament page
php artisan make:filament-page Settings

# Create Filament widget
php artisan make:filament-widget StatsWidget

# Create Filament user
php artisan make:filament-user
```

## 🔧 Configuration

### Database
Edit file `.env` untuk konfigurasi database:
```env
DB_CONNECTION=sqlite
DB_DATABASE=/path/to/database/database.sqlite

# Atau untuk MySQL
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=your_database
DB_USERNAME=your_username
DB_PASSWORD=your_password
```

### Filament
Konfigurasi Filament ada di:
- `config/filament.php` - Konfigurasi umum
- `app/Providers/Filament/` - Service providers
- `app/Filament/` - Resources, Pages, Widgets

## 📚 Documentation

- [Laravel Documentation](https://laravel.com/docs)
- [Filament Documentation](https://filamentphp.com/docs)
- [Laravel Bootcamp](https://bootcamp.laravel.com)

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## 📄 License

This project is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
