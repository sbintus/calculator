# Calculator API

A simple Node.js RESTful API for performing basic arithmetic operations (addition, subtraction, multiplication, division).

## Features
- Addition, subtraction, multiplication, and division endpoints
- Modular structure with controllers, models, and routes
- Docker support
- Unit tests

## Project Structure
```
api/
	controllers/         # Business logic for arithmetic operations
	models/              # Data models (if needed)
	routes.js            # API route definitions
public/
	index.html           # Frontend interface (if any)
	default.css          # Styles
server.js              # Main server entry point
Dockerfile             # Docker container configuration
test/                  # Unit and integration tests
```

## Getting Started

### Prerequisites
- Node.js (v14 or higher)
- npm

### Installation
1. Clone the repository:
	 ```sh
	 git clone https://github.com/sbintus/calculator.git
	 cd calculator
	 ```
2. Install dependencies:
	 ```sh
	 npm install
	 ```

### Running the Server
```sh
node server.js
```
The server will start on the default port (e.g., 3000).

### API Endpoints
- `POST /add`         - Add two numbers
- `POST /subtract`    - Subtract two numbers
- `POST /multiply`    - Multiply two numbers
- `POST /divide`      - Divide two numbers

Request body example:
```json
{
	"a": 5,
	"b": 3
}
```

### Running Tests
```sh
npm test
```

### Docker
To build and run with Docker:
```sh
docker build -t calculator-api .
docker run -p 3000:3000 calculator-api
```

## License
MIT

