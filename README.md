# Stripe Payment Processor - Monday.com Order Management Automation

This project automates Stripe payment processing and order management in Monday.com using Make.com.

It eliminates manual order entry by automatically creating, searching, and updating orders in Monday.com whenever a Stripe payment is received.

---

## 🚀 Overview

This automation captures Stripe payment data and processes it through multiple routes to:

- Watch for new Stripe events
- Search for existing orders in Monday.com
- Create new order items
- Update column values for existing orders
- Handle payment status changes
- Manage order fulfillment workflow

---

## ⚙️ How It Works

1. Stripe triggers when a payment event occurs
2. Router branches the flow based on event type
3. Monday.com searches for existing order by ID
4. Sleep module adds delay for processing
5. Conditional logic determines create vs update
6. New orders are created as items
7. Existing orders have column values updated
8. Multiple update modules handle different statuses

---

## 🛠️ Tools Used

- Make.com
- Stripe
- Monday.com (legacy)
- Router
- Sleep Module
- Search Module

---

## 📋 Modules Used

| Module | Service | Action |
|--------|---------|--------|
| Stripe 1 | Stripe | Watch Events (Trigger) |
| Router 6 | Make.com | Conditional Branching |
| Monday.com (legacy) 8 | Monday.com | Search Items in Board by Column Values |
| Sleep | Make.com | Delay processing |
| Monday.com (legacy) 3 | Monday.com | Create an Item (advanced) |
| Monday.com (legacy) 9 | Monday.com | Get an Item |
| Monday.com (legacy) 12 | Monday.com | Update Column Values |
| Monday.com (legacy) 15 | Monday.com | Update Column Values |

---

## 🔥 Key Features

- Real-time Stripe payment processing
- Duplicate order detection
- Automatic order creation in Monday.com
- Dynamic column value updates
- Sleep delay for data consistency
- Multi-route processing logic
- Handles multiple payment statuses

---

## 📸 Scenario Diagram

<img width="1341" height="579" alt="image" src="https://github.com/user-attachments/assets/2e9e796b-1f0c-4fe6-947d-15b2f5985813" />


*Complete workflow showing Stripe → Router → Monday.com order management*

---

## 🎯 Use Case

This system is ideal for:

- E-commerce businesses
- Subscription-based services
- Payment processing teams
- Order management operations
- Finance and accounting teams

---

## 📈 Benefits

- Saves hours of manual order entry
- Eliminates duplicate orders
- Real-time order tracking in Monday.com
- Automatic status updates
- Centralized payment data
- Reduces human errors

---

## 🔄 Data Flow
