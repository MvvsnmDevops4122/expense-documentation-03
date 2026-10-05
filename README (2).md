# Expense 3-Tier Architecture

## Project Overview

This project documents a **3-Tier Expense Application Architecture**
using AWS.

The application is divided into three main layers:

1.  **Frontend**
2.  **Backend**
3.  **Database**

The project also covers **Load Balancing, HTTP status codes, Backend
API, Nginx configuration, and MySQL setup**.

## Architecture

``` text
User / Browser
      |
      v
Load Balancer
      |
      v
Frontend Server
      |
      v
Backend API
      |
      v
MySQL Database
```

## Project Structure

  File                        Description
  --------------------------- ----------------------------------------
  `01-mysql.md`               MySQL database setup and configuration
  `02-backend.md`             Backend server setup
  `03-frontend.md`            Frontend server setup
  `04-lb.md`                  Load Balancer setup
  `05-http-status-codes.md`   HTTP status codes and their meanings
  `backend-api.md`            Backend API details
  `expense.conf`              Expense application configuration
  `lb.conf`                   Load Balancer configuration
  `three-tier-arch (1).png`   3-Tier architecture diagram

## Technologies Used

-   AWS EC2
-   MySQL
-   Node.js
-   Nginx
-   Load Balancer
-   Linux
-   HTTP / HTTPS
-   DNS

## 3-Tier Architecture

### 1. Frontend Tier

The frontend server serves the application to the user.

**Technology:** Nginx

### 2. Backend Tier

The backend handles application requests and business logic.

**Technology:** Node.js

### 3. Database Tier

The database stores application data.

**Technology:** MySQL

## Request Flow

When a user accesses the application:

``` text
Browser
   |
   v
Load Balancer
   |
   v
Frontend / Nginx
   |
   v
Backend API
   |
   v
MySQL
```

The response follows the reverse path back to the user.

## Learning Topics

This repository covers:

-   MySQL setup
-   Backend server setup
-   Frontend server setup
-   Load Balancer setup
-   Backend API
-   Nginx configuration
-   HTTP methods
-   HTTP status codes
-   3-Tier architecture
-   AWS EC2 communication

## Goal

The goal of this project is to understand how a **3-Tier application
works in AWS** and how the frontend, backend, database, and load
balancer communicate with each other.
