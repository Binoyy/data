
# Alloc8 : Official room allocation site of IIT Patna

This project is a room allocation system built with a **React** and **Tailwind CSS** frontend, an **Express.js** backend, and **Prisma** for database management. The system is ideal for room allocation in educational institutions or organizations, providing a streamlined interface for administrators and efficient room assignment processes.

## Prerequisites

- **Node.js** (v16+ recommended)
- **Microsoft Azure** account for app registration (required for client authentication setup)
- **Prisma** for ORM and database management
- **Netlify** for frontend deployment (optional but recommended)
- **PM2** for backend deployment

---

## Project Setup and Installation

### Clone the Repository
```sh
git clone https://github.com/your-username/room-allocation.git
cd room-allocation
```

### Frontend Setup (Client)
1. Register an application on [Microsoft Azure Portal](https://portal.azure.com/) and configure **OAuth**. Add the required credentials to `client/src/authConfig.js`.
2. Install client dependencies and start the development server:

    ```sh
    cd client
    npm install
    npm run dev
    ```

3. Open [http://localhost:5173](http://localhost:5173) to view it in the browser.

### Backend Setup (Server)
1. Install server dependencies and start the development server:

    ```sh
    cd server
    npm install
    npm run start
    ```

2. The server will run at [http://localhost:8800](http://localhost:8800).

### Database Setup
- For database migrations and schema updates, run:

    ```sh
    npx prisma migrate dev
    ```
- After changes to the Prisma schema, regenerate the client:

    ```sh
    npx prisma generate
    ```

---

## Contributing

Contributions are welcome! Here’s how you can help:
- **Issue Reporting**: Submit bug reports, suggestions, or feature requests using GitHub Issues.
- **Code Contributions**: Fork the repository, create a new branch, make changes, and submit a pull request.

For further details, check out the `CONTRIBUTING.md`.

## License

This project is licensed under the MIT License. See `LICENSE` for more information.

---
