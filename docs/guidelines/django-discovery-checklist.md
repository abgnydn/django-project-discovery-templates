# 🔍 Django App Discovery Documentation

## 0. 🚀 SETUP & GETTING STARTED DOCUMENTATION

> 📁 **Document findings in:** setup/

### 0.1 Initial Setup README

> 📁 **Document in:** setup/installation.md

Document the complete setup process:

- [ ] Python version requirements
- [ ] Virtual environment creation steps
- [ ] Dependency installation (`pip install -r requirements.txt`)
- [ ] Environment variables setup (.env file template)
- [ ] Database setup (creation, migrations)
- [ ] Initial data/fixtures if needed
- [ ] How to run development server
- [ ] How to access admin panel (create superuser steps)
- [ ] Any additional services needed (Redis, Celery, etc.)

### 0.2 Feature-Specific Usage Documentation

> 📁 **Document in:** features/[feature-name].md (use feature template)

For each major feature (like "creating new project"):

- [ ] What business process does this feature support?
- [ ] Step-by-step user workflow
- [ ] Required permissions/user roles
- [ ] Form validation rules
- [ ] What happens after successful submission?
- [ ] Error scenarios and handling
- [ ] Related database changes
- [ ] Any background processing triggered

## 1. 📋 PROJECT OVERVIEW

> 📁 **Document findings in:** project-overview.md (root of docs/)

### 1.1 Basic Information

- [ ] Project name and purpose
- [ ] When was this project created?
- [ ] Who were the original developers?
- [ ] What business problem does it solve?
- [ ] Current number of active users/transactions
- [ ] Is this customer-facing, internal tool, or API?

### 1.2 Repository Structure (Single App)

- [ ] List all top-level directories and their purpose
- [ ] Main Django project folder structure
- [ ] Single Django app structure and organization
- [ ] Document any non-Django components (scripts, configs, etc.)
- [ ] Frontend assets organization (static, templates)
- [ ] What files are in the root directory and what do they do?

## 2. 🔧 TECHNICAL STACK AUDIT

> 📁 **Document findings in:** setup/

### 2.1 Python Environment

> 📁 **Document in:** setup/environment.md

- [ ] Python version in use
- [ ] Virtual environment setup (venv, conda, etc.)
- [ ] requirements.txt or pyproject.toml contents
- [ ] Any version conflicts or outdated packages?
- [ ] Development vs production dependencies

### 2.2 Django Configuration

> 📁 **Document in:** setup/environment.md

- [ ] Django version
- [ ] Settings file structure (dev/prod/staging splits?)
- [ ] Environment variables used and where they're defined
- [ ] Secret management approach
- [ ] Debug mode settings for each environment

### 2.3 Database Setup

> 📁 **Document in:** setup/environment.md

- [ ] Database type (PostgreSQL, MySQL, SQLite?)
- [ ] Database connection configuration
- [ ] Migration status - are all migrations applied?
- [ ] Any custom migration issues or dependencies?
- [ ] Database backup/restore procedures

### 2.4 Frontend Technologies

> 📁 **Document in:** architecture/frontend.md

- [ ] jQuery version and usage patterns
- [ ] CSS framework (Bootstrap, custom CSS?)
- [ ] JavaScript bundling approach (Webpack, none?)
- [ ] Static file handling configuration
- [ ] Template engine usage (Django templates, Jinja2?)

## 3. 🏗️ APPLICATION ARCHITECTURE

> 📁 **Document findings in:** architecture/

### 3.1 Single Django App Analysis

> 📁 **Document in:** architecture/overview.md

- [ ] App name and primary purpose
- [ ] Models defined (with relationships)
- [ ] Views and their functionality
- [ ] URL patterns
- [ ] Templates used
- [ ] Static files organization
- [ ] Admin interface customizations
- [ ] Custom management commands
- [ ] Forms and their validation logic

### 3.2 Feature Breakdown

> 📁 **Document in:** features/[feature-name].md (use feature template)

For each major feature (e.g., "Create Project", "User Management", etc.):

- [ ] Feature name and business purpose
- [ ] Entry points (URLs that trigger this feature)
- [ ] Forms involved and their fields
- [ ] Models/database tables affected
- [ ] Templates and JavaScript involved
- [ ] Permissions required
- [ ] Success/error workflows
- [ ] Email notifications or side effects

### 3.3 URL Structure Analysis

> 📁 **Document in:** architecture/urls.md

- [ ] Main URL configuration (urls.py)
- [ ] How URLs are organized within the single app
- [ ] API endpoints vs web pages
- [ ] Authentication-protected routes
- [ ] Static file serving setup

### 3.4 Model Relationships

> 📁 **Document in:** architecture/models.md

- [ ] Draw/document the complete data model diagram
- [ ] Foreign key relationships
- [ ] Many-to-many relationships
- [ ] Custom model managers or methods
- [ ] Signal usage and where
- [ ] Model validation rules

### 3.5 View Layer Analysis

> 📁 **Document in:** architecture/views.md

- [ ] Function-based vs class-based views breakdown
- [ ] Authentication and permission patterns
- [ ] Form handling approaches
- [ ] AJAX endpoints and their purposes
- [ ] File upload handling
- [ ] Pagination implementation

## 4. 🎨 FRONTEND ARCHITECTURE

> 📁 **Document findings in:** architecture/frontend.md

### 4.1 Template Structure

- [ ] Base template hierarchy
- [ ] Template inheritance patterns
- [ ] Shared components/includes
- [ ] Template context processors
- [ ] Custom template tags and filters

### 4.2 JavaScript Organization

- [ ] How is jQuery code organized?
- [ ] Inline scripts vs external files
- [ ] AJAX call patterns and endpoints
- [ ] Form validation approaches
- [ ] DOM manipulation patterns
- [ ] Any conflicts or duplicate functionality?

### 4.3 CSS/Styling

- [ ] CSS file organization
- [ ] Responsive design implementation
- [ ] Browser compatibility requirements
- [ ] Any CSS preprocessing (SASS, LESS?)
- [ ] Icon fonts or SVG usage

## 5. 🔄 DATA FLOW DOCUMENTATION

> 📁 **Document findings in:** architecture/data-flow.md

### 5.1 Request/Response Patterns

- [ ] How does a typical user request flow through the system?
- [ ] Middleware usage and order
- [ ] Session handling
- [ ] Cookie usage
- [ ] Caching strategies

### 5.2 Form Processing

- [ ] How are forms defined and validated?
- [ ] File upload workflows
- [ ] Error handling patterns
- [ ] Success/failure user feedback

### 5.3 Business Logic Location

- [ ] Where is business logic implemented? (models, views, utils?)
- [ ] Any business rules that span multiple features?
- [ ] Calculation or processing logic
- [ ] External API integrations

## 6. ⚙️ CONFIGURATION MANAGEMENT

> 📁 **Document findings in:** setup/

### 6.1 Settings Analysis

> 📁 **Document in:** setup/environment.md

- [ ] All Django settings and their purposes
- [ ] Environment-specific configurations
- [ ] Third-party app configurations
- [ ] Custom settings variables

### 6.2 External Dependencies

> 📁 **Document in:** setup/environment.md

- [ ] External APIs or services used
- [ ] Authentication providers (OAuth, LDAP?)
- [ ] Email configuration
- [ ] File storage (local, S3, etc.)
- [ ] Logging configuration

## 7. 🧪 TESTING & QUALITY

> 📁 **Document findings in:** analysis/testing-quality.md

### 7.1 Current Testing State

- [ ] Existing test coverage
- [ ] Types of tests present (unit, integration, functional)
- [ ] Test runner configuration
- [ ] Mock usage patterns
- [ ] CI/CD setup

### 7.2 Code Quality Issues

- [ ] Linting setup (flake8, pylint, black?)
- [ ] Code style consistency
- [ ] Known bugs or issues
- [ ] Performance bottlenecks
- [ ] Security concerns

## 8. 🚀 DEPLOYMENT & INFRASTRUCTURE

> 📁 **Document findings in:** setup/

### 8.1 Deployment Process

> 📁 **Document in:** setup/deployment.md

- [ ] How is the application currently deployed?
- [ ] Server/hosting environment
- [ ] Web server configuration (nginx, Apache?)
- [ ] WSGI server setup (gunicorn, uWSGI?)
- [ ] SSL certificate handling

### 8.2 Environment Management

> 📁 **Document in:** setup/deployment.md

- [ ] Development setup process
- [ ] Staging environment availability
- [ ] Production deployment steps
- [ ] Database migration process in production
- [ ] Rollback procedures

## 9. 🏢 SINGLE APP SPECIFIC CONSIDERATIONS

> 📁 **Document findings in:** analysis/app-organization.md

### 9.1 Code Organization Within App

- [ ] How is business logic organized in the single app?
- [ ] Are there subdirectories for different concerns?
- [ ] How are utilities and helpers organized?
- [ ] Is there clear separation between different features?

### 9.2 Potential Splitting Opportunities

- [ ] Features that could become separate apps in the future
- [ ] Code that's getting too large for a single app
- [ ] Different business domains mixed together
- [ ] Reusable components that could be extracted

## 10. 🔧 REFACTORING OPPORTUNITIES

> 📁 **Document findings in:** analysis/refactoring-opportunities.md

### 10.1 Quick Wins

- [ ] Code that can be easily extracted
- [ ] Unused code that can be removed
- [ ] Simple optimizations
- [ ] Documentation that can be added immediately

### 10.2 Major Improvements Needed

- [ ] Features that should be split
- [ ] Code that needs complete rewrite
- [ ] Architecture changes required
- [ ] Performance improvements needed

## 11. ⚠️ RISK ASSESSMENT

> 📁 **Document findings in:** analysis/risk-assessment.md

### 11.1 Critical Dependencies

- [ ] What would break if changed?
- [ ] Single points of failure
- [ ] Undocumented assumptions
- [ ] Legacy code that nobody understands

### 11.2 Technical Debt

- [ ] Outdated packages or patterns
- [ ] Workarounds that need proper solutions
- [ ] Missing error handling
- [ ] Scalability concerns

## 12. 👥 TEAM KNOWLEDGE TRANSFER

> 📁 **Document findings in:** team-knowledge.md (root of docs/)

### 12.1 Learning Requirements

- [ ] Django concepts you need to learn for this project
- [ ] Python patterns used that are unfamiliar
- [ ] Business domain knowledge needed
- [ ] External tools/services to understand

### 12.2 Documentation Gaps

- [ ] What documentation is missing entirely?
- [ ] What existing docs are outdated?
- [ ] What tribal knowledge needs to be captured?
- [ ] Who can provide missing information?

---

## 📚 HOW TO USE THIS TEMPLATE

1. **📋 Use this as your roadmap** - Check off items as you investigate them
2. **📁 Document findings in the specified files** - Each section tells you exactly where to put your discoveries
3. **📸 Take screenshots/diagrams** - Visual documentation is crucial for complex relationships
4. **⏰ Set a deadline** - Force yourselves to complete this in 1-2 weeks max
5. **🔄 Review regularly** - As you learn more, come back and update answers

## 🛠️ ADDITIONAL TOOLS TO HELP

- **🎨 Django Extensions** - Install `django-extensions` for model visualization: `python manage.py graph_models -a -o models.png`
- **🔍 Code analysis tools** - Use `prospector` or `bandit` to identify code quality issues
- **📊 Dependency visualization** - Use `pydeps` to see import relationships

## 🚨 RED FLAGS TO WATCH FOR

- 🔄 Apps importing from each other circularly
- 🌊 Business logic scattered across multiple layers
- 💾 Hard-coded values everywhere
- ❌ Missing error handling
- 🧪 No tests for critical functionality

## ✅ COMPLETION CHECKLIST

- [ ] 📁 All documentation files created in proper folders
- [ ] 🔍 All sections above completed
- [ ] 👥 Code walkthrough with someone familiar done
- [ ] 💻 Development environment successfully set up
- [ ] 🧪 Can run all tests successfully
- [ ] 🚀 Can deploy to staging environment
- [ ] 📞 Emergency contacts and escalation identified
- [ ] 💾 Backup and recovery procedures understood
