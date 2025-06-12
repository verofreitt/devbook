# DevBook Project

A social media platform for developers built with Go (backend) and React (frontend). The project consists of two main parts:
- API (RESTful backend service)
- WebApp (Frontend application)

## Project Structure
```
.
├── api/         # Go backend service
└── webapp/      # React frontend application
```

## Requirements

### API
- Go 1.19+
- MySQL 8.0+
- Environment variables set in `.env` file

### WebApp
- Node.js 16+
- NPM or Yarn
- Environment variables set in `.env` file

## Getting Started

### Setting up the API

1. Navigate to the API directory:
```bash
cd api
```

2. Create a `.env` file with the following variables:
```env
DB_USER=your_db_user
DB_PASSWORD=your_db_password
DB_NAME=devbook
API_PORT=5000
SECRET_KEY=your_jwt_secret
```

3. Install dependencies:
```bash
go mod tidy
```

4. Run the API:
```bash
go run main.go
```

The API will be available at `http://localhost:5000`

### Setting up the WebApp

1. Navigate to the WebApp directory:
```bash
cd webapp
```

2. Create a `.env` file with:
```env
REACT_APP_API_URL=http://localhost:5000
```

3. Install dependencies:
```bash
npm install
```

4. Start the development server:
```bash
npm start
```

The application will be available at `http://localhost:3000`

## Features

- User authentication (login/register)
- User profiles
- Posts creation and interaction
- Following system
- Feed with posts from followed users
- Real-time updates

## Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.