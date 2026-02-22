SmartInventory Full-Stack Application

Overview

This is a full-stack Product Inventory Management web application built using:

React (Frontend)
FastAPI (Backend)
SQLAlchemy (ORM)
PostgreSQL (Database)

The application allows users to perform complete CRUD operations (Create, Read, Update, Delete) on products.

Features
Add new products
View product list
Update product details
Delete products
RESTful API architecture
Data validation using Pydantic
Database interaction using SQLAlchemy ORM
PostgreSQL integration
CORS enabled for frontend-backend communication

Tech Stack
Frontend
React
Axios
CSS

Backend
FastAPI
SQLAlchemy
Pydantic
Uvicorn

Database
PostgreSQL

Architecture

User → React → Axios (HTTP Request) → FastAPI → Pydantic Validation → SQLAlchemy → PostgreSQL → Response → React UI Update

The frontend communicates with the backend using REST APIs. FastAPI validates incoming data using Pydantic schemas and interacts with PostgreSQL through SQLAlchemy ORM.


API Endpoints
| Method | Endpoint       | Description      |
| ------ | -------------- | ---------------- |
| GET    | /products      | Get all products |
| POST   | /products      | Add new product  |
| PUT    | /products/{id} | Update product   |
| DELETE | /products/{id} | Delete product   |


Database Schema

Product Table:
id (Primary Key)
name (String)
description (String)
price (Float)
quantity (Integer)

