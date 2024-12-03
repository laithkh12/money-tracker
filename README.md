# Money Tracker

Money Tracker is a web application designed to manage your personal finances by tracking income and expenses in real time. This project is built with React for the front end and Node.js with Express for the back end.

## Features

- Add income and expense transactions with details like description, date, and price.
- View all past transactions.
- Dynamic balance calculation.
- REST API integration for seamless data management.

## Tech Stack

- **Frontend**: React
- **Backend**: Node.js, Express
- **Database**: MongoDB
- **Environment Variables**: `dotenv`

## Setup Instructions

### Prerequisites

Ensure you have the following installed on your system:

- Node.js
- npm or yarn
- MongoDB instance
- A `.env` file configured with the following variables:
```plaintext
REACT_APP_API_URL=http://localhost:4040/api
MONGO_URL=<your-mongodb-connection-string>
```
### Steps to Run the Project
1. **Clone the Repository**
```bash
 git clone https://github.com/<your-username>/money-tracker.git
 cd money-tracker
```
2. **Install Dependencies**
```bash
cd src
yarn add .
```
3. **Run the Backend**
```bash
nodemon index.js
```
```plaintext
The backend will run on http://localhost:4040.
```
4. **Run the Frontend**
```bash
yarn start
```

## API Endpoints
- GET /api/transactions
  - Fetches all transactions.
- POST /api/transaction
  - Adds a new transaction.
  - Body:
  ```json
  {
  "name": "New transaction name",
  "description": "Transaction details",
  "datetime": "2024-12-03T12:00:00",
  "price": 100
  }
  ```
  
## Future Improvements
- User authentication for personalized tracking.
- Data visualization with charts.
- Mobile responsiveness.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request for any changes you'd like to make.

## License
This project is licensed under the MIT License.
