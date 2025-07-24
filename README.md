# NewClaudeOnRailsProject

A modern Rails 8 application built with ClaudeOnRails for enhanced development experience.

## Overview

This is a full-stack Rails application that leverages ClaudeOnRails with a swarm of specialized agents for different aspects of Rails development. Each agent has specific expertise and works in designated directories to collaborate on implementing features across all application layers.

## Technology Stack

- **Rails Version**: 8.0.2
- **Ruby Version**: 3.4.3
- **Database**: SQLite3
- **Frontend**: Turbo + Stimulus + Tailwind CSS
- **Asset Pipeline**: Propshaft
- **Web Server**: Puma
- **Testing**: Minitest
- **Development**: ClaudeOnRails 0.2.0 with agent swarm

## Key Features

- Modern Rails 8 architecture
- Turbo/Stimulus for interactive frontend
- Tailwind CSS for styling
- Solid Cache, Queue, and Cable for background processing
- ClaudeOnRails integration for AI-assisted development
- Docker support with Kamal deployment
- Comprehensive test suite

## Getting Started

### Prerequisites

- Ruby 3.4.3
- Rails 8.0.2
- SQLite3

### Installation

1. Clone the repository
```bash
git clone <repository-url>
cd new-claude-on-rails-project
```

2. Install dependencies
```bash
bundle install
```

3. Setup database
```bash
rails db:create
rails db:migrate
rails db:seed
```

### Development

Start the development server:
```bash
bin/dev
```

This will start:
- Rails server on http://localhost:3000
- Tailwind CSS watcher

### Testing

Run the test suite:
```bash
rails test
```

For system tests:
```bash
rails test:system
```

### Code Quality

Run code linting:
```bash
bundle exec rubocop
```

Run security analysis:
```bash
bundle exec brakeman
```

## ClaudeOnRails Integration

This project uses ClaudeOnRails with a specialized agent swarm defined in `claude-swarm.yml`. The agents include:

- **Models Agent**: ActiveRecord models, migrations, and database optimization
- **Controllers Agent**: Rails controllers, routing, and request handling
- **Views Agent**: Rails views, layouts, partials, and asset pipeline
- **Tests Agent**: Minitest testing, factories, and test coverage
- **Jobs Agent**: Background jobs, ActiveJob, and async processing
- **Stimulus Agent**: Stimulus.js controllers and Turbo integration
- **DevOps Agent**: Deployment, Docker, CI/CD, and production configuration

## Deployment

This application is configured for deployment using Kamal. See `config/deploy.yml` for deployment configuration.

## Contributing

1. Follow Rails conventions and best practices
2. Write tests for all new functionality
3. Use strong parameters in controllers
4. Keep models focused with single responsibilities
5. Extract complex business logic to service objects
6. Ensure proper database indexing for foreign keys and queries

## License

This project is available as open source.
