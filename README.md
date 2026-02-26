<p align="center">
  <a href="README.ja.md">日本語</a> | <a href="README.zh.md">中文</a> | <a href="README.es.md">Español</a> | <a href="README.fr.md">Français</a> | <a href="README.hi.md">हिन्दी</a> | <a href="README.it.md">Italiano</a> | <a href="README.pt-BR.md">Português (BR)</a>
</p>

<p align="center">
  <img src="https://raw.githubusercontent.com/mcp-tool-shop-org/brand/main/logos/pocket-ledger/readme.png" width="400" alt="Pocket Ledger">
</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-blue.svg" alt="MIT License"></a>
  <a href="https://mcp-tool-shop-org.github.io/pocket-ledger/"><img src="https://img.shields.io/badge/Landing_Page-live-blue" alt="Landing Page"></a>
</p>

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

Built by <a href="https://mcp-tool-shop.github.io/">MCP Tool Shop</a>
