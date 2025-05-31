# Employee Management System

A Spring Boot application for managing employees, departments and projects with MySQL database integration.

## 🎯 Overview

This Employee Management System is a RESTful web application built with Spring Boot that allows you to manage organizational data including employees, departments and projects. The system provides CRUD operations and maintains relationships between different entities.

## ✨ Features

- **Department Management**: Create and manage organizational departments
- **Employee Management**: Handle employee records with department associations
- **Project Management**: Manage projects and assign employees
- **Database Integration**: MySQL database with JPA/Hibernate
- **RESTful APIs**: Clean REST endpoints for all operations
- **Entity Relationships**: Proper mapping between departments, employees and projects

## 🛠 Tech Stack

- **Backend**: Spring Boot 3.5.0
- **Database**: MySQL
- **ORM**: Spring Data JPA / Hibernate
- **Build Tool**: Maven
- **Java Version**: 17
- **Testing**: JUnit 5

## 📋 Prerequisites

Before running this application, make sure you have the following installed:

- Java 17 or higher
- Maven 3.6+ (or use the included Maven wrapper)
- MySQL 8.0+
- Git

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/employee-management-system.git
   cd employee-management-system
   ```

2. **Navigate to the system directory**
   ```bash
   cd system
   ```

## 🗄 Database Setup

1. **Create MySQL Database**
   ```sql
   CREATE DATABASE systemdb;
   ```

## 🗃 Database Schema

### Department Entity
- `dept_id` (Primary Key) - Department ID
- `name` - Department name (Not Null)
- `established` - Date established

### Employee Entity
- `empNo` (Primary Key) - Employee number
- `name` - Employee name
- `age` - Employee age
- `salary` - Employee salary
- `gender` - Employee gender
- `department` - Foreign key to Department

### Project Entity
- `id` (Primary Key) - Project ID
- `name` - Project name
- `totalCost` - Total project cost

### Relationships
- **Department ↔ Employee**: One-to-Many (One department has many employees)
- **Employee ↔ Project**: Many-to-Many (Employees can work on multiple projects)

## 🚀 Screenshots

![Screenshot 2025-05-31 170228](https://github.com/user-attachments/assets/51da4276-b169-4706-b372-e82a8aa9807b)
