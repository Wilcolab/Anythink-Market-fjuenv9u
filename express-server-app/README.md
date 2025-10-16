# Express Server Application

This is a simple Express server application that listens on port 8001. It is set up to use Nodemon for automatic code reloading during development.

## Project Structure

```
express-server-app
├── src
│   └── app.js          # Entry point of the application
├── package.json        # Project configuration and dependencies
├── yarn.lock           # Dependency version lock file
├── Dockerfile          # Instructions to build the Docker image
└── README.md           # Project documentation
```

## Getting Started

To get started with this project, follow the instructions below.

### Prerequisites

Make sure you have [Node.js](https://nodejs.org/) and [Yarn](https://yarnpkg.com/) installed on your machine.

### Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   cd express-server-app
   ```

2. Install the dependencies:
   ```
   yarn install
   ```

### Running the Server

To run the server in development mode with automatic reloading, use the following command:

```
yarn start
```

The server will start and listen on [http://localhost:8001](http://localhost:8001).

### Building the Docker Image

To build the Docker image for the application, run the following command in the project root:

```
docker build -t express-server-app .
```

### Running the Docker Container

After building the image, you can run the Docker container with:

```
docker run -p 8001:8001 express-server-app
```

The server will be accessible at [http://localhost:8001](http://localhost:8001).

## License

This project is licensed under the MIT License.