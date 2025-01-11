# Roxiler-MERN-Stack-Project
# Transaction Management System

A web application for managing product transactions. This project includes APIs for database initialization, transaction statistics, and visualization (bar chart and pie chart) along with a responsive frontend for data display and interaction.

# Features
Fetch and initialize database with third-party JSON data.

List transactions with search and pagination.

**Display statistics for selected months, including:**

Total sales amount.

Number of sold and unsold items.

# Visualize transaction data using:

Bar charts (price range vs. item count).

Pie charts (category vs. item count).

Responsive UI for data exploration and interaction.


# Tech Stack

Backend: Node.js, Express.js, MongoDB

Frontend: React.js, Chart.js, Axios

Third-Party API: https://s3.amazonaws.com/roxiler.com/product_transaction.json

# Directory Structure
![image](https://github.com/user-attachments/assets/570d3fe8-805d-4b0b-9511-6b4d51718aa9)

# APIs
# 1. Initialize Database
Endpoint: GET /api/seed
Description: Fetches data from a third-party API and seeds the database.
# List Transactions
Endpoint: GET /api/transactions
Query Parameters:
month (required): Month name (e.g., March).
search (optional): Search term for title, description, or price.
page (optional): Page number (default: 1).
perPage (optional): Records per page (default: 10).
# 3. Transaction Statistics
Endpoint: GET /api/statistics
Query Parameters: month (required).
# 4. Bar Chart Data
Endpoint: GET /api/bar-chart
Query Parameters: month (required).
# 5. Pie Chart Data
Endpoint: GET /api/pie-chart
Query Parameters: month (required).
# 6. Combined Data
Endpoint: GET /api/combined
Query Parameters: month (required).
