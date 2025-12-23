# Chalo Ride-Booking & Sharing System

**Chalo Ride-Booking & Sharing System** is a **console-based C++ application** that simulates a real-world ride-booking platform.  
The system allows customers to book rides using different vehicle types, apply promo codes, choose payment methods, and view detailed billing along with ride history.

This project demonstrates strong usage of **Object-Oriented Programming (OOP)** concepts such as inheritance, polymorphism, abstraction, and encapsulation.

---

## Project Overview
The application enables customers to:
- Book **private or shared rides**
- Select suitable vehicles based on distance
- Apply promo codes and payment discounts
- View a complete bill breakdown
- Maintain a ride history
- Provide feedback and ratings

The system is designed to closely resemble real ride-booking services while running entirely in a **terminal environment**.

---

## System Design

### Vehicle Classes
- **Vehicle (Abstract Base Class)**
  - Defines pure virtual functions for fare calculation

- **Derived Classes**
  - `Car`
  - `Motorcycle`
  - `Scooty`
  - `Auto`

Each vehicle calculates fare based on:
- Base fare
- Distance travelled
- Time taken

---

### Ride Class
Handles all ride-related functionality:

#### Ride Input
- Choose ride type: **Private / Shared**
- Enter travel distance
- Select a suitable vehicle
- Apply promo code
- Choose payment method: **Online / Offline**

#### Fare Calculation
- Calculates base, distance, and time fare
- Applies **shared ride discount (30%)**
- Applies **promo discounts**
  - Flat ₹50
  - 20% discount
  - 25% discount (up to ₹60)
- Applies **online payment discount**

#### Billing & Summary
- Displays detailed bill breakdown
- Shows applied discounts
- Displays total payable amount
- Stores ride details in history

#### Ride History
- Maintains up to **100 previous rides**
- Allows users to view past ride summaries

---

### Customer Class
Handles customer-related information:

- Accepts customer details:
  - Name
  - Email
  - Phone number
- Performs **input validation**
- Allows customers to:
  - Give ratings (out of 5)
  - Provide written feedback
- Displays customer profile and review

---

## Program Flow (`main()` Function)

1. Customer registration
2. Menu-driven interaction:
   - Book a ride
   - View ride summary
   - View ride history
   - Provide feedback (optional)
3. Option to book another ride or exit

---

## Key Features
- Object-oriented design using C++
- Multiple vehicle options
- Private and shared ride support
- Promo code and payment discounts
- Detailed fare calculation
- Ride history management
- Customer reviews and ratings
- User-friendly console interaction

---

## Tech Stack
- **Language:** C++
- **Concepts Used:**  
  - OOP (Inheritance, Polymorphism, Abstraction)  
  - STL (Vectors / Arrays)  
  - Input validation  

---

## Use Cases
- Understanding real-world OOP application design  
- Learning fare calculation logic  
- Simulating ride-booking systems  
- Academic and learning projects in C++  

