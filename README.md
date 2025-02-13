# AI Terraform Module Generator Frontend

The web interface for the AI Terraform Module Generator project. This frontend service provides a user-friendly interface for managing Terraform modules and interacting with the AI generation capabilities.

## Features

- User authentication and role-based access control
- Module repository management
- AI module generation interface
- Terraform Registry Protocol compatibility
- Module version management
- Repository integration with GitHub

## Prerequisites

- Node.js 18+
- PostgreSQL 14+
- Docker and Docker Compose

## Quick Start

1. Clone the repository:
```bash
git clone https://github.com/HappyPathway/ai-terraform-module-generator-frontend.git
```

2. Create and configure environment variables:
```bash
cp .env.example .env
# Edit .env with your configuration
```

3. Start the development environment:
```bash
docker compose up -d
```

4. Access the application at http://localhost:5000

## Configuration

### Environment Variables

- `DB_HOST`: PostgreSQL host
- `DB_PORT`: PostgreSQL port
- `DB_NAME`: Database name
- `DB_USER`: Database user
- `DB_PASSWORD`: Database password
- `SECRET_KEY`: Flask secret key
- `BACKEND_URL`: URL of the backend service
- `ADMIN_EMAIL`: Email for the initial admin user

## Development

### Local Development Setup

1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Run database migrations:
```bash
flask db upgrade
```

3. Start the development server:
```bash
flask run
```

### Running Tests

```bash
pytest
```

## Project Structure

```
├── app/                # Application package
│   ├── __init__.py    # Flask app initialization
│   ├── models/        # Database models
│   ├── routes/        # API routes
│   ├── templates/     # Jinja2 templates
│   └── static/        # Static assets
├── migrations/        # Database migrations
├── tests/            # Test suite
└── docker/           # Docker configuration
```

## API Documentation

The frontend service implements the Terraform Registry Protocol for module discovery and download. See [API Documentation](docs/api.md) for details.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to your branch
5. Create a pull request

## Related Repositories

- [Main Project](https://github.com/HappyPathway/ai-terraform-module-generator)
- [Backend Service](https://github.com/HappyPathway/ai-terraform-module-generator-backend)
- [Infrastructure](https://github.com/HappyPathway/ai-terraform-module-generator-infrastructure)

## License

MIT License - see [LICENSE](LICENSE) for details