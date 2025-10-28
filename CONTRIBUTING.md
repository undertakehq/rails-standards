# Contributing to Undertake HQ Rails Standards

First off, thank you for considering contributing to undertakehq-rails-standards! It's people like you that make this gem such a great tool.

## Code of Conduct

This project and everyone participating in it is governed by the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/). By participating, you are expected to uphold this code.

## How Can I Contribute?

### Reporting Bugs

Before creating bug reports, please check the issue list as you might find out that you don't need to create one. When you are creating a bug report, please include as many details as possible:

- **Use a clear and descriptive title**
- **Describe the exact steps which reproduce the problem** in as many details as possible
- **Provide specific examples to demonstrate the steps**
- **Describe the behavior you observed after following the steps**
- **Explain which behavior you expected to see instead and why**
- **Include screenshots or animated GIFs if possible**
- **Include your environment details** (Ruby version, Rails version, OS, etc.)

### Suggesting Enhancements

Enhancement suggestions are tracked as GitHub issues. When creating an enhancement suggestion, please include:

- **Use a clear and descriptive title**
- **Provide a step-by-step description of the suggested enhancement** in as many details as possible
- **Provide specific examples to demonstrate the steps**
- **Describe the current behavior** and **the suggested new behavior**
- **Explain why this enhancement would be useful**

### Pull Requests

- Fill in the pull request template
- Follow the Ruby style guide (enforced by RuboCop)
- Include appropriate test cases for new functionality
- Update documentation as needed
- End all files with a newline
- Use meaningful commit messages

## Development Setup

1. Fork the repository
2. Clone your fork:
   ```bash
   git clone https://github.com/your-username/rails-standards.git
   cd rails-standards
   ```
3. Add the upstream repository:
   ```bash
   git remote add upstream https://github.com/undertakehq/rails-standards.git
   ```
4. Create a feature branch:
   ```bash
   git checkout -b feature/your-feature-name
   ```
5. Install dependencies:
   ```bash
   bundle install
   ```

## Development Workflow

### Running Tests

```bash
# Run all tests
bundle exec rspec

# Run a specific test file
bundle exec rspec spec/path/to/test_spec.rb

# Run tests matching a pattern
bundle exec rspec -e "pattern"

# Run tests with coverage
bundle exec rspec --require spec_helper --format progress
```

### Code Style

This project uses RuboCop for code style enforcement. Before committing:

```bash
# Check for style violations
bundle exec rubocop

# Auto-fix violations
bundle exec rubocop -A
```

### Security

Check for vulnerable dependencies:

```bash
bundle exec bundler-audit
```

## Testing Guidelines

- Write tests for all new functionality
- Ensure all tests pass before submitting a pull request
- Use descriptive test names that explain what is being tested
- Group related tests using `describe` and `context` blocks
- Mock external dependencies appropriately
- Aim for high code coverage

### Test Structure

```ruby
describe 'FeatureName' do
  context 'when condition is met' do
    it 'does something specific' do
      # Arrange
      # Act
      # Assert
    end
  end
end
```

## Commit Message Guidelines

- Use the imperative mood ("add feature" not "added feature")
- Limit the first line to 72 characters
- Reference issues and pull requests liberally after the first line
- Consider starting the commit message with a type/scope:
  - `feat:` for new features
  - `fix:` for bug fixes
  - `docs:` for documentation
  - `style:` for formatting/style changes
  - `refactor:` for code refactoring
  - `test:` for test additions/changes

Example:
```
feat: add new validation helper

Add a new helper method for validating user input across
models. This provides a consistent way to validate data
and improves code reusability.

Closes #123
```

## Pull Request Process

1. Update the README.md with details of any changes to the interface
2. Update the CHANGELOG.md with notes on your changes
3. Ensure all tests pass:
   ```bash
   bundle exec rspec
   ```
4. Ensure code style compliance:
   ```bash
   bundle exec rubocop
   ```
5. Ensure no security vulnerabilities:
   ```bash
   bundle exec bundler-audit
   ```
6. Request review from maintainers
7. Address any feedback or requested changes

## Questions or Need Help?

- Check existing [issues](https://github.com/undertakehq/rails-standards/issues)
- Open a new issue with your question

## Recognition

Contributors will be recognized in the project's CHANGELOG and README as appropriate.

## License

By contributing to rails-standards, you agree that your contributions will be licensed under its MIT License.

Thank you for contributing! 🎉
