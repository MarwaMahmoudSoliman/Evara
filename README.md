EvAra E-commerce 🛍️

![image](https://github.com/user-attachments/assets/18c680e6-eb59-4bc7-92e9-c7da76974937)# EvAra E-commerce 🛒
Project Overview

EvAra is a full-stack ASP.NET Core online marketplace for fashion enthusiasts. Designed with modern aesthetics and robust functionality, it empowers sellers to showcase products while offering customers a seamless shopping experience – complete with secure payments and order tracking.

Live Demo: https://evara-demo.example.com
🌟 Key Features
User Management

    Role-based access (Admin, Seller, Customer) via ASP.NET Core Identity

    Email confirmation & password recovery using SendGrid

    Profile management with avatar uploads

E-Commerce Core

    🛒 Product catalog with filters (category, price, ratings)

    ⏳ Real-time inventory tracking

    💳 Stripe/PayPal integration for secure payments

    📦 Order history with shipment tracking

Dashboards

    📊 Admin panel for user management & analytics

    🏪 Seller portal to manage products/orders

    ❤️ Wishlists & saved carts for customers

Tech Highlights

    EF Core Code-First with SQL Server

    Repository pattern & dependency injection

    Responsive UI with Bootstrap 5 + custom themes

🛠️ Tech Stack
Layer	Technology
Frontend	Razor Pages, AJAX, Bootstrap 5
Backend	ASP.NET Core MVC, Web API
Database	SQL Server + EF Core (Code-First)
Payment	Stripe & PayPal APIs
Deployment	Docker + Azure App Service
⚡ Getting Started
Prerequisites

    Visual Studio 2022+

    .NET 8 SDK

    SQL Server

    Stripe/PayPal test keys

    SendGrid API key for emails

Setup

    Clone the repo
    bash

git clone https://github.com/MarwaMahmoudSoliman/Evara.git
cd Evara

Configure appsettings.json
json

"ConnectionStrings": {
  "DefaultConnection": "Server=(localdb)\\mssqllocaldb;Database=EvaraDb;"
},
"Stripe": {
  "PublishableKey": "pk_test_...",
  "SecretKey": "sk_test_..."
},
"SendGrid": {
  "ApiKey": "SG.your-api-key"
}

Run migrations
bash

Update-Database

Launch
bash

    dotnet run

    Visit https://localhost:5001

🚀 Deployment

Deployed via Azure App Service with CI/CD pipeline.
Deploy to Azure
📜 License

MIT License - See LICENSE.md




