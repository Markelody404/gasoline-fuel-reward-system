# Gasoline Fuel Reward System

A system for gasoline stations that records customer fuel transactions, calculates reward points, 
and manages a loyalty rewards program. Customers earn points based on the liters (or amount) of fuel 
purchased, which can be accumulated and redeemed later.  

---

## Features
- **Transaction Recording**  
  Records each purchase with details such as:
  - Ticket number
  - Fuel type
  - Amount
  - Points earned
  - Date of transaction
  - Customer ID  

- **Customer Management**  
  - Assigns unique customer IDs and registration dates  
  - Tracks total accumulated points  
  - (Future) Edit and delete options for better management  

- **Loyalty Rewards**  
  - Points calculated automatically (e.g., 1% of transaction amount)  
  - Stored in the customer’s profile  

- **Database Structure**  
  - **customers** table → ID, name, registration date, total points  
  - **transactions** table → linked to customers, stores transaction details  

- **Demo Data Generator**  
  - `create_sample_db.py` creates a sample `database.db`  
  - Randomized customers and transaction histories for testing  

- **Database Tools**  
  - Backup script for safe storage  
  - Migration script for schema updates  

- **Web Integration (Flask)**  
  - Displays transactions, rewards, and reports  
  - (Planned) Dashboard with charts and summaries  

---

## Project Purpose
This system helps gasoline stations improve customer retention by rewarding loyalty.  
It provides owners with clear insights into transactions and customer activity while giving customers 
a reason to keep coming back.  

---

## Requirements
- Python 3.x  
- SQLite3  
- Flask (for web integration)  
- Other dependencies: listed in `requirements.txt`  

---

## How to Use
1. Clone the repository.  
2. Run `create_sample_db.py` to generate the sample database.  
3. Start the Flask app (`app.py`).  
4. Access the system via your web browser.  

---

## File Overview
- **create_sample_db.py** → Generates `database.db` with demo data  
- **migrate_database.py** → Handles schema changes and backups  
- **app.py** → Main Flask web application  
- **requirements.txt** → Python dependencies  

---

## Status
- Core database and loyalty system implemented  
- Transaction and customer management in progress  
- Dashboard and visual reports planned  
