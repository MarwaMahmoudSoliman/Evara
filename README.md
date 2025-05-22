EvAra E-commerce 🛍️

![image](https://github.com/user-attachments/assets/18c680e6-eb59-4bc7-92e9-c7da76974937)# EvAra E-commerce 🛒
Project Overview

EvAra is a full-stack ASP.NET Core online marketplace for fashion enthusiasts. Designed with modern aesthetics and robust functionality, it empowers sellers to showcase products while offering customers a seamless shopping experience – complete with secure payments and order tracking.

🌟 Key Features
User Management


     ASP.NET Core Identity (register, login, email confirmation, forgot password, reset password).
    
    External logins (Google, Facebook, Microsoft Account).

    Role-based access (Admin, Seller, Customer) via ASP.NET Core Identity

    Email confirmation & password recovery

    Profile management with avatar uploads

E-Commerce Core

    🛒 Product catalog with filters (category, price, ratings)

    ⏳ Real-time inventory tracking

    💳 Stripe integration for secure payments

    📦 Order history with shipment tracking

Dashboards

    📊 Admin panel for user management & analytics

    🏪 Seller portal to manage products/orders

    ❤️ Wishlists & saved carts for customers

Tech Highlights

    EF Core Code-First with SQL Server

    Repository pattern & dependency injection

    Responsive UI with Bootstrap 5 + custom themes

UML Diagrams

  class, sequence,use case  and Interaction diagrams link:https://drive.google.com/drive/folders/181sdzldFozvp8k09ajallaj_v4QQDuva

![image](https://github.com/user-attachments/assets/18c680e6-eb59-4bc7-92e9-c7da76974937)# EvAra E-commerce 🛒
🛠️ Tech Stack
Layer	Technology
Frontend	Razor Pages, AJAX, Bootstrap 5
Backend	ASP.NET Core MVC, Web API
Database	SQL Server + EF Core (Code-First)
Payment	Stripe  APIs


🏗️ Architecture & Design
Clean Architecture Layers
Layer	Responsibilities	Key Components
Domain	Business logic & core entities	Product, Order, User aggregates
Application	Use cases & interfaces	IProductRepository, OrderService
Infrastructure	External implementations	EF Core,tripe API
Presentation	UI & API endpoints	MVC Controllers, Razor Pages


⚡ Getting Started
Prerequisites

    Visual Studio 2022+

    .NET 9 SDK

    SQL Server

    Stripe test keys

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
}EmailSettings{
  "FromEmail": "your-email@gmail.com",
  "SmtpServer": "smtp.gmail.com",
  "Port": 587,
  "EnableSSL": true
}

Run migrations
bash

Update-Database

Launch
bash

    dotnet run

    Visit https://localhost:5001

Contributing

    Fork the repo
    Create a feature branch (git checkout -b feat/my-new-feature)
    Commit your changes (git commit -m 'Add new feature')
    Push to the branch (git push origin feat/my-new-feature)
    Open a Pull Request

Troubleshooting

    Migrations failing? Ensure DefaultConnection is correct and SQL Server is running.
    External logins not working? Verify OAuth credentials and redirect URIs in Google/Facebook developer consoles.
    Stripe/PayPal errors? Check sandbox keys.

License

This project is licensed under the MIT License. See LICENSE for details.
Acknowledgments

    ASP.NET Core MVC Documentation
    Entity Framework Core
   stripe API


