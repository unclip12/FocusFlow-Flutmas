# App Structure - FocusFlow Flutmas

The project follows a **Feature-First Clean Architecture** approach.

## Directory Layout

```text
lib/
├── core/               # App-wide utilities, themes, constants
│   ├── theme/          # Material 3 theme definitions
│   ├── constants/      # App constants (colors, spacing, etc.)
│   └── utils/          # Helper functions
├── features/           # Feature-based modules
│   ├── task/           # Task Management Feature
│   │   ├── data/       # Hive models, adapters, repositories
│   │   ├── domain/     # Entities, use cases
│   │   └── presentation/ # UI, Riverpod providers
│   ├── timer/          # Focus Timer Feature
│   └── dashboard/      # Analytics & Stats Feature
└── main.dart           # App entry point & initialization
```

## Layer Responsibilities

### 1. Data Layer
- **Models**: Hive-annotated classes for local storage.
- **Data Sources**: Direct interaction with Hive boxes.
- **Repositories**: Implementation of domain repository interfaces.

### 2. Domain Layer
- **Entities**: Pure Dart classes representing business objects.
- **Use Cases**: Specific business logic (e.g., `CalculateSrsNextDate`).
- **Repository Interfaces**: Abstract definitions for data access.

### 3. Presentation Layer
- **Providers**: Riverpod state management logic.
- **Screens**: Full-page widgets.
- **Widgets**: Reusable UI components.
