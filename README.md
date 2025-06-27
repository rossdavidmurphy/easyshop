# EasyShop E-Commerce API

## Overview

**EasyShop** is a Java-based e-commerce backend application built using **Spring Boot** and **MySQL**. This project is the final capstone in the Pluarlsight Java Development program, focusing on real-world backend development tasks like bug fixing, feature implementation, and database integration. 

This API powers the Version 2 backend of the EasyShop online store.

---

## 📦 Project Structure

- **Backend:** Spring Boot RESTful API  
- **Database:** MySQL  
- **Authentication:** JWT-based  
- **Frontend:** Pre-built demo web app (provided in starter code)

  <img width="1439" alt="easyshop front end interface" src="https://github.com/user-attachments/assets/2ac338b3-3fba-4ffa-8cd0-17b9450de88a" />


---

## 📋 Requirements & Features

- User registration & login  
- Browse products by category  
- Search/filter products  
- Checkout and cart functionality (on frontend)

---

# 🛠️ Development Tasks

## Phase 1: CategoriesController

- Implement missing CRUD methods  
- Use `@PreAuthorize("hasRole('ADMIN')")` for security on `POST`, `PUT`, `DELETE`

---

## Phase 2: Fix Bugs in ProductsController

### Bug 1: Broken Search/Filter

- Fix logic errors in `GET /products` search

**Query Parameters:**

- `cat (int)`: Category ID  
- `minPrice (BigDecimal)`: Minimum price  
- `maxPrice (BigDecimal)`: Maximum price  
- `color (String)`: Product color

---

### Bug 2: Duplicate Products on Update

- Fix incorrect `UPDATE` logic that inserts instead of updates  
- Ensure updating a product modifies the record rather than duplicating it

---

## 🧪 Testing

- Manual testing: Postman  
- Automated testing: JUnit 5

**Test coverage includes:**

- Bug fixes  
- New endpoint functionality  
- Authentication flows

  <img width="712" alt="Screenshot 2025-06-26 at 11 21 40 PM" src="https://github.com/user-attachments/assets/2e340920-e31b-4914-83d2-464e6acd541e" />
  

  <img width="709" alt="Screenshot 2025-06-26 at 11 22 16 PM" src="https://github.com/user-attachments/assets/51fc456f-0219-4484-826e-91e1504c062a" />



