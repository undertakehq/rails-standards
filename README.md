# Undertake Rails Standards

A Ruby gem containing general conventions and standards for Rails projects. This gem provides a set of best practices, patterns, and configurations that help maintain consistency across Rails applications.

## Features

- Standardized Rails conventions and patterns
- Reusable configuration templates
- Common Rails extensions and helpers
- Best practices for Rails development

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'undertakehq-rails-standards'
```

And then execute:

```bash
$ bundle install
```

Or install it yourself as:

```bash
$ gem install undertakehq-rails-standards
```

## Usage

After installing the gem, create an initializer in your Rails application:

```ruby
# config/initializers/rails_standards.rb

RailsStandards.configure do |config|
  # Configuration options will be available here
end
```

For detailed usage instructions and available features, see the [documentation](docs/).

## Development

### Setup

Clone the repository and install dependencies:

```bash
git clone https://github.com/undertakehq/rails-standards.git
cd rails-standards
bundle install
```

### Running Tests

```bash
bundle exec rspec
```

Run a specific test file:

```bash
bundle exec rspec spec/path/to/test_spec.rb
```

### Code Quality

Run linting:

```bash
bundle exec rubocop
```

Auto-fix linting issues:

```bash
bundle exec rubocop -A
```

Check for vulnerable dependencies:

```bash
bundle exec bundler-audit
```

## Contributing

We welcome contributions from the community! Please read our [CONTRIBUTING.md](CONTRIBUTING.md) guide for details on our code of conduct and the process for submitting pull requests.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Code of Conduct

This project and everyone participating in it is governed by the [Contributor Covenant Code of Conduct](https://www.contributor-covenant.org/version/2/1/code_of_conduct/). By participating, you are expected to uphold this code.

## Support

For issues, questions, or suggestions, please [open an issue](https://github.com/undertakehq/rails-standards/issues) on GitHub.
