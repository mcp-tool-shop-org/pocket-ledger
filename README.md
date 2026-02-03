# PocketLedger

A local-first personal finance and budget tracking app for Windows. Clean, simple, and privacy-focused.

## Philosophy

- **Local-first**: Your financial data stays on your device. No cloud sync required.
- **Privacy by design**: Zero telemetry, zero external connections unless you opt-in.
- **Envelope budgeting**: Proven methodology that assigns every dollar a job.
- **Goal-oriented**: Focus on what you're saving for, not just what you're spending.

## Features (Planned)

- [ ] Transaction tracking with categories
- [ ] Envelope-based budgeting system
- [ ] Savings goals with visual progress
- [ ] Recurring transaction management
- [ ] Visual spending insights and reports
- [ ] Multi-account support
- [ ] CSV import/export
- [ ] Dark/light theme support

## Tech Stack

- **.NET 8** - Modern, performant runtime
- **WinUI 3 / Windows App SDK** - Native Windows 11 experience
- **SQLite** - Local, portable database
- **Clean Architecture** - Maintainable, testable layers

## Project Structure

```
src/
├── PocketLedger.Domain/        # Core entities and business rules
├── PocketLedger.Application/   # Use cases and application logic
├── PocketLedger.Infrastructure/# Data persistence, external services
└── PocketLedger.Desktop/       # WinUI 3 presentation layer
tests/
├── PocketLedger.Domain.Tests/
├── PocketLedger.Application.Tests/
└── PocketLedger.Infrastructure.Tests/
```

## Development

### Prerequisites

- Windows 10/11
- Visual Studio 2022 (17.8+) or VS Code with C# Dev Kit
- .NET 8 SDK
- Windows App SDK

### Building

```bash
dotnet build
```

### Running Tests

```bash
dotnet test
```

## License

MIT License - See [LICENSE](LICENSE) for details.

## Contributing

Contributions welcome! Please read our contributing guidelines before submitting PRs.

---

Built with care by [mcp-tool-shop](https://github.com/mcp-tool-shop-org)
