
# CaterQuest

CaterQuest is a distributed catering service platform that bridges the gap between families seeking budget-friendly catering and local vendors/homemakers offering high-quality services.

## Features

- Real-time chat using WebSockets (Flask-SocketIO)
- Vendor listings with search by name, location, and ratings
- Secure user authentication with hashed passwords
- Order placement and status updates
- Ratings and reviews for vendors
- Caching using `shelve` for faster data retrieval
- Retry mechanism using `tenacity` library
- Connection pooling for optimized database usage

## System Design

- **Scalability**: Caching and connection pooling reduce load on the backend and database.
- **Fault Tolerance**: Data replication, retry logic, and caching ensure high availability.
- **Event-Driven Architecture**: Enables real-time communication between vendors and customers.

## Technology Stack

- Frontend: HTML, JavaScript
- Backend: Python, Flask, Flask-SocketIO
- Database: MySQL
- Caching: Python Shelve
- Other Libraries: Tenacity

## Performance

- Cache hit retrieval is ~16x faster than direct DB fetch.
- 10,000 GET requests improved from 66s to 60s using connection pooling.
- Chat latency under 50ms.

## License

This project is for academic and learning purposes.

## Author

- Dhruti Dobariya,
- M.E. Computer Science,
- Bits Pilani, Hyderabad Campus
