# Jobs API
Jobs API is a Node.js application that provides authentication endpoints (register and login) and CRUD operations for managing jobs. The authentication routes are public, while the job-related routes are protected.

## Getting Started

### Prerequisites

- Node.js (v12 or higher)
- npm (Node Package Manager)
- MongoDB (Make sure you have a running MongoDB instance)

### Installation

1. Clone the repository:```bash git clone https://github.com/Kalutu/jobs-api ```
2. Change into the project directory: ```bash cd jobs-api```
3. Install dependencies: ```bash npm install ```

### Configuration
Create a .env file in the root directory with the following content:
- PORT=your port
- MONGO_URI=your connection string
- JWT_SECRET=your-secret-key

## API Endpoints

### Public Routes:

- `POST /api/v1/auth/register`: Register a new user.
- `POST /api/v1/auth/login`: Authenticate and log in a user.

### Protected Routes:

- `POST /api/v1/jobs`: Create a new job.
- `GET /api/v1/jobs`: Get all jobs.
- `GET /api/v1/jobs/:id`: Get a specific job by ID.
- `PUT /api/v1/jobs/:id`: Update a job by ID.
- `DELETE /api/v1/jobs/:id`: Delete a job by ID.

## Security Measures
- **Helmet:** Helps secure your Express application by setting various HTTP headers.
- **CORS:** Enables Cross-Origin Resource Sharing to control which domains can access your API.
- **XSS-Clean:** Protects against Cross-Site Scripting (XSS) attacks by sanitizing user input.
- **Rate Limiting:** Limits the number of requests to protect against abuse.

## Contributing
We welcome contributions! If you find a bug or have a feature request, please open an issue or submit a pull request.
