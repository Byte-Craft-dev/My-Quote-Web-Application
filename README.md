# MyQuote Rails Application

A comprehensive quote management web application built with Ruby on Rails 7, featuring secure user authentication, administrative moderation capabilities, and role-based access control. The application implements a complete backend architecture with an ERD-based relational database design.

## 🚀 Features

- **Secure Authentication System**
  - User registration and login with BCrypt password encryption
  - Session management and secure password handling
  - Protected routes and authorization

- **Admin Moderation**
  - Administrative dashboard for content oversight
  - Quote approval and rejection workflow
  - User management capabilities

- **Quote Management**
  - Create, read, update, and delete quotes
  - Categorization and tagging system
  - Search and filter functionality

- **Role-Based Access Control**
  - User roles: Admin, Moderator, and Standard User
  - Permission-based feature access
  - Hierarchical authorization system

- **RESTful Architecture**
  - Rails MVC design pattern
  - ActiveRecord ORM for database operations
  - Clean and maintainable codebase

## 🛠 Technical Stack

- **Framework:** Ruby on Rails 7.0.8.7
- **Ruby Version:** 3.2.2
- **Database:** SQLite3 (Development), PostgreSQL-ready for production
- **Authentication:** BCrypt 3.1.7
- **Frontend:** Stimulus, Turbo, Importmap
- **Testing:** Capybara, Selenium WebDriver

## 📋 Prerequisites

Before you begin, ensure you have the following installed:

- Ruby 3.2.2
- Rails 7.0.8.7
- SQLite3
- Node.js (for asset compilation)
- Bundler 2.5.6

## 🔧 Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/YOUR_USERNAME/myquote-rails-app.git
   cd myquote-rails-app
   ```

2. **Install dependencies**
   ```bash
   bundle install
   ```

3. **Database setup**
   ```bash
   # Create the database
   rails db:create
   
   # Run migrations
   rails db:migrate
   
   # Seed the database (optional)
   rails db:seed
   ```

4. **Start the Rails server**
   ```bash
   rails server
   ```

5. **Visit the application**
   
   Open your browser and navigate to `http://localhost:3000`

## 🗄 Database Schema

The application uses an ERD-based relational database design with the following core models:

- **Users** - Authentication and profile information
- **Quotes** - Quote content and metadata
- **Categories** - Quote categorization
- **Roles** - User role definitions
- **Permissions** - Role-based permissions

## 🎯 Usage

### For Regular Users
1. Register for an account
2. Browse and search quotes
3. Submit quotes for moderation
4. Manage your submitted quotes

### For Moderators
1. Review submitted quotes
2. Approve or reject submissions
3. Edit quote categories

### For Administrators
1. Full moderation capabilities
2. User management and role assignment
3. System configuration and oversight

## 📁 Project Structure

```
myquote-rails-app/
├── app/
│   ├── controllers/    # Request handling and business logic
│   ├── models/         # ActiveRecord models and associations
│   ├── views/          # ERB templates
│   └── helpers/        # View helpers
├── config/
│   ├── routes.rb       # Application routing
│   └── database.yml    # Database configuration
├── db/
│   ├── migrate/        # Database migrations
│   └── schema.rb       # Current database schema
└── test/               # Test suite
```

## 🔐 Security Features

- BCrypt password hashing
- CSRF protection
- SQL injection prevention through ActiveRecord
- Session security with encrypted cookies
- Role-based authorization

## 🧪 Running Tests

```bash
# Run all tests
rails test

# Run specific test file
rails test test/models/user_test.rb

# Run with verbose output
rails test --verbose
```

## 🚀 Deployment

For production deployment:

1. Set environment variables:
   ```bash
   RAILS_ENV=production
   SECRET_KEY_BASE=your_secret_key
   ```

2. Use PostgreSQL for production database

3. Precompile assets:
   ```bash
   rails assets:precompile
   ```

4. Run migrations:
   ```bash
   rails db:migrate RAILS_ENV=production
   ```

## 📝 Configuration

Key configuration files:

- `config/database.yml` - Database settings
- `config/routes.rb` - Application routing
- `config/environments/` - Environment-specific settings

## 🤝 Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Your Name**
- GitHub: [@Byte-Craft-dev](https://github.com/Byte-Craft-dev)
- LinkedIn: [Tharushi Karawgoda](http://www.linkedin.com/in/tharushi-navodya-)

## 🙏 Acknowledgments

- Ruby on Rails community
- Rails guides and documentation
- Contributors and testers

