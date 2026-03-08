# 📈 Price Comparator Java Backend App  
A backend application for comparing product prices across multiple stores.    
Built with Java, Spring Boot, and Gradle, this project processes CSV product data and provides endpoints for alerts, baskets, discounts, and product information.  

## 🛠 Tools & Technologies
IDE: IntelliJ IDEA  
Language: Java (OpenJDK 17.0.15)  
Build Tool: Gradle (Kotlin DSL)  
Framework: Spring Boot  
CSV Handling: BufferedReader (no external libraries)  
Frontend: HTML, JavaScript  

## 📁 Project Structure
src/<br>
 ├── main/<br>
 │  ├── java/<br>
 │  │  └── org.App/<br>
 │  │    ├── Controllers/<br>
 │  │    │  ├── AlertsController<br>
 │  │    │  ├── BasketController<br>
 │  │    │  ├── DiscountsController<br>
 │  │    │  ├── HomeController<br>
 │  │    │  └── ProductsController<br>
 │  │    ├── Loaders/<br>
 │  │    │  ├── DiscountsLoader<br>
 │  │    │  └── ProductsLoader<br>
 │  │    ├── Models/<br>
 │  │    │  ├── Alerts<br>
 │  │    │  ├── Discounts<br>
 │  │    │  └── Products<br>
 │  │    ├── Service/<br>
 │  │    │  ├── AlertsService<br>
 │  │    │  ├── DiscountsService<br>
 │  │    │  └── ProductsService<br>
 │  │    └── Main<br>
 │  └── resources/<br>
 │    ├── data/<br>
 │    │  ├── kaufland_2025-05-01.csv<br>
 │    │  ├── kaufland_2025-05-08.csv<br>
 │    │  ├── kaufland_discounts_2025-05-01.csv<br>
 │    │  ├── kaufland_discounts_2025-05-08.csv<br>
 │    │  ├── lidl_2025-05-01.csv<br>
 │    │  ├── lidl_2025-05-08.csv<br>
 │    │  ├── lidl_discounts_2025-05-01.csv<br>
 │    │  ├── lidl_discounts_2025-05-08.csv<br>
 │    │  ├── mega_2025-05-20.csv<br>
 │    │  ├── mega_2025-05-23.csv<br>
 │    │  ├── mega_discounts_2025-05-20.csv<br>
 │    │  ├── mega_discounts_2025-05-23.csv<br>
 │    │  ├── profi_2025-05-01.csv<br>
 │    │  ├── profi_2025-05-08.csv<br>
 │    │  ├── profi_discounts_2025-05-01.csv<br>
 │    │  └── profi_discounts_2025-05-08.csv<br>
 │    └── static/<br>
 │      ├── add-alert.html<br>
 │      ├── basket.html<br>
 │      └── delete-alert.html<br>
 └────/ 

## 🚀 Getting Started
1. Download the project  
 Go to the master branch → click Code → Download ZIP  
2. Open in IntelliJ  
 Unzip the project  
 Right-click the folder → Open Folder as IntelliJ IDEA Project  
 Click Trust Project if prompted  
3. Set JDK  
 Click SetupSDK in the top-right yellow ribbon  
 Select ms-17 (OpenJDK 17.0.15)  
4. Load Gradle  
 Click Load in the bottom-right corner to load Gradle build files  
5. Run the Application  
 Navigate to src/main/java/org.App/Main  
 Click the green Run arrow  
6. Access the Backend  
 Open your browser at: http://localhost:8080/home  
 Example endpoints: /products/store/{storeName}   → storeName: lidl | kaufland | profi | mega/products/category/{categoryName}  
 Replace {storeName} or {categoryName} with your desired value  

## 📌 Assumptions
IntelliJ IDEA and OpenJDK 17 must be installed  
Tested with ms-17, JDK version 17.0.15  

## 📊 Features
View product lists per store  
Monitor discounts and promotions  
Manage product alerts  
Handle baskets with products  
Simple HTML/JS frontend for interaction  

## ⚙ How CSVs Are Used
CSV files are loaded via BufferedReader without external libraries  
Products and discounts are parsed and stored in memory  
Supports multiple stores with versioned CSVs  

## 🔗 Live Links (Local)
Home: /home  
Products: /products/store/{storeName}  
Alerts: /alerts  
Basket: /basket  
Discounts: /discounts  
