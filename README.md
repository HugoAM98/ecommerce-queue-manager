# 🚀 Ecommerce Queue Management System

![Project Banner](https://via.placeholder.com/1200x400/2D3748/FFFFFF?text=Ecommerce+Queue+System)  
*A scalable queue system for e-commerce (like IKEA Click & Collect), featuring real-time updates and priority management.*

[![Laravel](https://img.shields.io/badge/Laravel-FF2D20?style=for-the-badge&logo=laravel&logoColor=white)](https://laravel.com)
[![Vue.js](https://img.shields.io/badge/Vue.js-4FC08D?style=for-the-badge&logo=vuedotjs&logoColor=white)](https://vuejs.org)
[![Redis](https://img.shields.io/badge/Redis-DC382D?style=for-the-badge&logo=redis&logoColor=white)](https://redis.io)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg?style=for-the-badge)](LICENSE)

## 🌟 Features

✅ **Real-time queue updates** using WebSockets (Laravel Echo + Soketi)  
✅ **Priority queues** (VIP/normal customers) with Redis  
✅ **Admin dashboard** with live metrics  
✅ **Mobile-friendly** Vue 3 frontend  
✅ **RESTful API** for integration with mobile apps  

## 📦 Prerequisites

- PHP 8.1+
- Composer
- Node.js 16+
- MySQL 5.7+
- Redis

## 🛠️ Installation

```bash
# Clone the repository
git clone https://github.com/your-username/ecommerce-queue-system.git
cd ecommerce-queue-system

# Install PHP dependencies
composer install

# Install JavaScript dependencies
npm install

# Create environment file
cp .env.example .env

# Generate application key
php artisan key:generate

# Run database migrations
php artisan migrate --seed

# Start the development servers
php artisan serve
npm run dev

# In another terminal, start Soketi for WebSockets
soketi start
