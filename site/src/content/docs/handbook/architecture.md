---
title: Architecture
description: Clean Architecture layers in Pocket Ledger — domain, application, infrastructure, and UI.
sidebar:
  order: 3
---

Pocket Ledger follows Clean Architecture with four distinct layers.

## Domain layer

Core entities and business rules with no external dependencies:

- **Account** — checking, savings, credit, cash
- **Transaction** — individual financial entries with category and envelope assignment
- **Envelope** — budget categories with allocated amounts
- **Goal** — savings targets with deadlines and progress

Domain events propagate state changes without coupling layers.

## Application layer

Use cases that orchestrate domain logic:

- CreateTransaction, TransferFunds, AllocateBudget
- Service interfaces define boundaries
- DTOs carry data between layers without leaking domain types

## Infrastructure layer

Persistence and external concerns:

- SQLite database with repository pattern
- Entity Framework or raw ADO.NET for data access
- File system operations for import/export

## Desktop layer (UI)

WinUI 3 presentation with MVVM:

- **CommunityToolkit.Mvvm** for observable properties, commands, and messaging
- **Microsoft.Extensions.DependencyInjection** for service registration
- Views bind to ViewModels, ViewModels call Application services

## Testing strategy

| Layer | Test type | Dependencies |
|-------|-----------|-------------|
| Domain | Pure unit tests | None |
| Application | Unit tests | Mocked repositories |
| Infrastructure | Integration tests | In-memory SQLite |
