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

- **Web Integration (**
