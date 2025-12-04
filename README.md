# LMS (Learning Management System) Backend API

<p align="center">
  <img src="https://img.shields.io/badge/NestJS-E0234E?style=for-the-badge&logo=nestjs&logoColor=white" alt="NestJS" />
  <img src="https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white" alt="TypeScript" />
  <img src="https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white" alt="PostgreSQL" />
  <img src="https://img.shields.io/badge/JWT-000000?style=for-the-badge&logo=jsonwebtokens&logoColor=white" alt="JWT" />
</p>

## 📋 Description

A robust Learning Management System (LMS) backend API built with NestJS, designed to provide comprehensive educational platform functionality. This API serves as the backbone for managing users, courses, enrollments, and other core LMS features.

## ✨ Features

- **User Management**: Complete CRUD operations for user accounts
- **Authentication & Authorization**: JWT-based authentication with Passport
- **Database Integration**: TypeORM with PostgreSQL support
- **Validation**: Class-validator for input validation and transformation
- **Security**: Password hashing with bcrypt
- **Modular Architecture**: Clean, scalable NestJS module structure
- **Testing**: Comprehensive unit and e2e testing setup

## 🛠 Tech Stack

- **Framework**: [NestJS](https://nestjs.com/)
- **Language**: TypeScript
- **Database**: PostgreSQL with TypeORM
- **Authentication**: JWT with Passport
- **Validation**: class-validator & class-transformer
- **Password Hashing**: bcrypt
- **Testing**: Jest
- **Linting**: ESLint with Prettier

## 🚀 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/a-3isa/lms.git
   cd lms
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Environment Setup**
   Create a `.env` file in the root directory and configure the following variables:
   ```env
   PORT=3000
   DATABASE_HOST=localhost
   DATABASE_PORT=5432
   DATABASE_USERNAME=your_username
   DATABASE_PASSWORD=your_password
   DATABASE_NAME=lms_db
   JWT_SECRET=your_jwt_secret
   ```

4. **Database Setup**
   Ensure PostgreSQL is running and create the database specified in your environment variables.

## 🏃 Running the Application

```bash
# development
npm run start:dev

# production mode
npm run start:prod

# debug mode
npm run start:debug
```

The API will be available at `http://localhost:3000` (or the port specified in your `.env`).

## 🧪 Testing

```bash
# unit tests
npm run test

# e2e tests
npm run test:e2e

# test coverage
npm run test:cov

# test in watch mode
npm run test:watch
```

## 📚 API Endpoints

### User Management
- `POST /user` - Create a new user
- `GET /user` - Get all users
- `GET /user/:id` - Get user by ID
- `PATCH /user/:id` - Update user by ID
- `DELETE /user/:id` - Delete user by ID

### Authentication (Future Implementation)
- `POST /auth/login` - User login
- `POST /auth/register` - User registration
- `POST /auth/refresh` - Refresh JWT token

## 📁 Project Structure

```
lms/
├── src/
│   ├── app.controller.ts
│   ├── app.module.ts
│   ├── app.service.ts
│   ├── main.ts
│   └── user/
│       ├── dto/
│       │   ├── create-user.dto.ts
│       │   └── update-user.dto.ts
│       ├── entities/
│       │   └── user.entity.ts
│       ├── user.controller.ts
│       ├── user.module.ts
│       ├── user.service.ts
│       └── user.service.spec.ts
├── test/
│   ├── app.e2e-spec.ts
│   └── jest-e2e.json
├── package.json
├── tsconfig.json
└── README.md
```

## 🔧 Development

```bash
# linting
npm run lint

# formatting
npm run format

# build
npm run build
```

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the UNLICENSED License.

## 📞 Contact

Repository: [https://github.com/a-3isa/lms](https://github.com/a-3isa/lms)

For questions or support, please open an issue in the GitHub repository.
