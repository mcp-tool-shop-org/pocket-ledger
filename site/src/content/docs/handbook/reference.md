---
title: Reference
description: Technical reference for Pocket Ledger — tech stack, building, and project structure.
sidebar:
  order: 4
---

## Tech stack

| Component | Technology |
|-----------|-----------|
| Runtime | .NET 8 |
| UI Framework | WinUI 3 / Windows App SDK |
| Database | SQLite |
| MVVM | CommunityToolkit.Mvvm |
| DI | Microsoft.Extensions.DependencyInjection |

## Project structure

```
src/
├── PocketLedger.Domain/        # Core entities and business rules
├── PocketLedger.Application/   # Use cases and application logic
├── PocketLedger.Infrastructure/ # Data persistence, external services
└── PocketLedger.Desktop/       # WinUI 3 presentation layer
tests/
├── PocketLedger.Domain.Tests/
├── PocketLedger.Application.Tests/
└── PocketLedger.Infrastructure.Tests/
```

## Prerequisites

- Windows 10 or Windows 11
- Visual Studio 2022 (17.8+) or VS Code with C# Dev Kit
- .NET 8 SDK
- Windows App SDK

## Building

```bash
dotnet build
dotnet test
```

## Security

- All data stored locally in SQLite
- No telemetry, no analytics, no network connections
- No credential storage
- See [SECURITY.md](https://github.com/mcp-tool-shop-org/pocket-ledger/blob/main/SECURITY.md) for vulnerability reporting
