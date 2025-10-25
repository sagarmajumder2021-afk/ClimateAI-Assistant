# Contributing to ClimateAI Assistant

Thank you for your interest in contributing to ClimateAI Assistant! 🌍

## 🚀 Getting Started

### Prerequisites
- Python 3.9+
- Docker & Docker Compose
- Node.js 16+ (for frontend)
- Git

### Development Setup
```bash
# Clone the repository
git clone https://github.com/sagarmajumder2021-afk/ClimateAI-Assistant.git
cd ClimateAI-Assistant

# Copy environment file
cp .env.example .env

# Start development environment
docker-compose up -d

# Run tests
docker-compose exec api pytest tests/
```

## 🛠️ Development Workflow

### 1. Create a Branch
```bash
git checkout -b feature/your-feature-name
```

### 2. Make Your Changes
- Follow the existing code style
- Add tests for new functionality
- Update documentation as needed

### 3. Test Your Changes
```bash
# Run unit tests
pytest tests/ -v

# Run linting
flake8 api/
black api/ --check

# Run type checking
mypy api/
```

### 4. Commit Your Changes
```bash
git add .
git commit -m "feat: add your feature description"
```

Follow conventional commits:
- `feat:` New feature
- `fix:` Bug fix
- `docs:` Documentation changes
- `test:` Test additions/changes
- `refactor:` Code refactoring
- `chore:` Maintenance tasks

### 5. Push and Create Pull Request
```bash
git push origin feature/your-feature-name
```

## 📝 Code Style Guidelines

### Python
- Follow PEP 8
- Use type hints
- Write docstrings for functions and classes
- Maximum line length: 127 characters

### Example:
```python
from typing import Dict, Any

def process_climate_data(data: Dict[str, Any]) -> Dict[str, float]:
    """
    Process raw climate data and extract features.
    
    Args:
        data: Raw climate data dictionary
        
    Returns:
        Processed features dictionary
    """
    # Implementation
    pass
```

## 🧪 Testing Guidelines

### Writing Tests
- Write tests for all new functionality
- Include both positive and negative test cases
- Test edge cases and error conditions
- Aim for >90% test coverage

### Test Structure
```python
class TestClimateForecasting:
    """Test cases for climate forecasting."""
    
    def test_forecast_generation(self):
        """Test successful forecast generation."""
        # Test implementation
        pass
    
    def test_forecast_error_handling(self):
        """Test error handling in forecasting."""
        # Test implementation
        pass
```

## 📚 Documentation

### Code Documentation
- Add docstrings to all functions and classes
- Include parameter descriptions and return types
- Provide usage examples where helpful

### API Documentation
- Update OpenAPI specs for new endpoints
- Include request/response examples
- Document error codes and messages

## 🎯 Types of Contributions

### 🐛 Bug Fixes
- Fix existing issues
- Add tests to prevent regression
- Update documentation if needed

### ✨ New Features
- Add new climate data sources
- Implement new ML models
- Enhance edge computing capabilities
- Improve frontend interface

### 📖 Documentation
- Improve existing documentation
- Add tutorials and examples
- Fix typos and clarify instructions

### 🧪 Testing
- Add missing tests
- Improve test coverage
- Add integration tests

## 🔄 Adding New Components

### New API Endpoint
1. Define Pydantic models in `api/app/schemas/`
2. Implement endpoint in `api/app/api/`
3. Add tests in `tests/api/`
4. Update OpenAPI documentation

### New ML Model
1. Implement model in `ml/models/`
2. Add training script in `ml/trainer/`
3. Create inference service in `ml/predictor/`
4. Add model tests in `tests/ml/`

### New Edge Feature
1. Implement in `edge/gateway/`
2. Add MQTT topic handling
3. Implement local inference logic
4. Add edge tests in `tests/edge/`

## 🚀 Deployment Contributions

### Docker Support
- Improve Dockerfiles
- Optimize container sizes
- Add docker-compose configurations

### Kubernetes
- Add K8s manifests
- Create Helm charts
- Improve deployment strategies

### CI/CD
- Enhance GitHub Actions workflows
- Add security scanning
- Improve test automation

## 📋 Pull Request Guidelines

### Before Submitting
- [ ] Tests pass locally
- [ ] Code follows style guidelines
- [ ] Documentation is updated
- [ ] Commit messages are clear
- [ ] Branch is up to date with main

### Pull Request Template
```markdown
## Description
Brief description of changes

## Type of Change
- [ ] Bug fix
- [ ] New feature
- [ ] Documentation update
- [ ] Performance improvement

## Testing
- [ ] Tests added/updated
- [ ] All tests pass
- [ ] Manual testing completed

## Checklist
- [ ] Code follows style guidelines
- [ ] Self-review completed
- [ ] Documentation updated
- [ ] No breaking changes
```

## 🤝 Community Guidelines

### Be Respectful
- Use inclusive language
- Be constructive in feedback
- Help others learn and grow

### Communication
- Ask questions if unclear
- Provide context in issues and PRs
- Be patient with review process

## 🎉 Recognition

Contributors will be recognized in:
- README.md contributors section
- Release notes for significant contributions
- Special thanks in documentation

## 📞 Getting Help

- 📧 Email: sagarm.work@gmail.com
- 💬 GitHub Issues: For bugs and feature requests
- 📖 Documentation: Check existing docs first

## 🌟 Areas We Need Help

- **Climate Data Integration**: Adding new data sources
- **ML Models**: Improving forecasting accuracy
- **Edge Computing**: Optimizing edge inference
- **Frontend**: Enhancing user experience
- **Documentation**: Tutorials and guides
- **Testing**: Increasing test coverage
- **Security**: Security audits and improvements

Thank you for contributing to ClimateAI Assistant! 🌍🚀