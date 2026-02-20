# FocusFlow Flutmas

FocusFlow Flutmas is a high-performance, beautiful, and offline-first mobile application built with Flutter. It is a migration of the original FocusFlow web application.

## 🤖 AI HANDOVER PROTOCOL (MANDATORY)

If you are an AI agent taking over this project, you **MUST** follow these steps before proceeding:

1.  **Read `PLAN.md`**: Understand the overall roadmap and architectural decisions.
2.  **Read `PROGRESS.md`**: Check the current status and what was last implemented.
3.  **Update Progress**: After completing any task, you **MUST** update `PROGRESS.md` and `PLAN.md` to reflect the changes.
4.  **Document Requirements**: Any new user demands or creative ideas mentioned in chat must be added to the "User Requirements" section in `PLAN.md`.

## Tech Stack
- **Framework:** Flutter
- **State Management:** Riverpod (`flutter_riverpod`)
- **Local Database:** Hive (`hive_flutter`)
- **Architecture:** Clean Architecture (Data, Domain, Presentation)
- **Design:** Material 3 with custom animations

## Project Structure
- `lib/core/`: Common utilities, themes, and constants.
- `lib/features/`: Feature-based modules (task, timer, dashboard).
  - `data/`: Models, adapters, and repositories.
  - `domain/`: Entities and use cases.
  - `presentation/`: Riverpod providers, screens, and widgets.
- `reference_focusflow/`: Original React/TypeScript source code for logic reference.

## Setup Instructions
1. Ensure Flutter is installed.
2. Run `flutter pub get`.
3. Run `flutter pub run build_runner build` to generate Hive adapters and Riverpod code.
4. Run the app using `flutter run`.
