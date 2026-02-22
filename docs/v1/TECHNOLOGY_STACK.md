# Technology Stack - FocusFlow Flutmas

## Core Framework
- **Flutter**: Latest stable version for cross-platform mobile development.
- **Dart**: Modern, sound-typed language.

## State Management
- **Riverpod (flutter_riverpod)**: For robust, testable, and scalable state management.
- **Riverpod Generator**: To reduce boilerplate and ensure type safety.

## Local Database (Offline-First)
- **Hive / Hive Flutter**: Lightweight and blazing fast NoSQL database.
- **Hive Generator**: For automatic adapter generation.

## Architecture
- **Clean Architecture**: 
  - **Data Layer**: Repositories, Data Sources, Models (Hive).
  - **Domain Layer**: Entities, Use Cases, Repository Interfaces.
  - **Presentation Layer**: Riverpod Providers, Screens, Widgets.

## UI & UX
- **Material 3**: Latest design system from Google.
- **Animations**: 
  - `flutter_animate` for easy, performant animations.
  - Custom `AnimationController` for complex interactions.
- **Charts**: `fl_chart` for productivity analytics.

## Utilities
- **get_it**: For service location (if needed alongside Riverpod).
- **uuid**: For unique ID generation.
- **intl**: For internationalization and date formatting.
