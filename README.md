# Waste2Taste

Waste2Taste is a Flutter-based food rescue application that helps users discover surplus and near-expiry food, map nearby food partners, and place orders while supporting a sustainable food ecosystem.

The application is designed around a food rescue movement that connects restaurants, food vendors, and customers through a mobile experience focused on saving food, reducing waste, and creating a more responsible consumption flow.

## Features

- User authentication and profile flows
- Food product and partner listing
- Food request and product order flow
- Map view for nearby rescue locations
- Order tracking and profile management
- Localized UI for Arabic and English
- Dark and light theme support
- Firebase integration and secure app configuration

## Tech Stack

- Flutter
- Dart
- Firebase
- Google Maps
- Flutter Bloc
- GoRouter
- Dio and repository/service architecture
- Localization and theme management

## Project Structure

```text
lib/
  Features/
    auth/
    home/
    map/
    orders/
    products/
    profile/
    report/
    splash/
  core/
    constants/
    cubits/
    database/
    enums/
    errors/
    extensions/
    functions/
    l10n/
    mappers/
    services/
    theme/
    usecase/
    utils/
    widgets/
```

## Architecture

The project follows a feature-first layered architecture inspired by Clean Architecture and Flutter feature modularization.

Each feature in the application is organized into a structure that mirrors the app domain:

```text
Features/
  feature_name/
    data/
    domain/
    presentation/
```

- data: models, data sources, API handling, repository implementations, and DTO/model conversion logic
- domain: entities, use cases, contracts and business rules
- presentation: screens, widgets, Cubits/Blocs, and UI state handling

The shared application services and utilities are centralized under the core folder, including:

- constants and enums
- theme and localization
- API and storage services
- route configuration and dependency injection
- reusable widgets and helpers

State management is handled mainly through Flutter Bloc/Cubit, navigation is organized with GoRouter, and dependency injection is prepared through the service locator setup in the core utilities layer.

## Getting Started

### Install dependencies

```sh
flutter pub get
```

### Run the application

```sh
flutter run
```

### Run tests

```sh
flutter test
```

## Configuration

This project uses Flutter localization and Firebase configuration entries. Make sure the Firebase configuration file and required environment values are configured correctly before running the app.

## App Goal

The main goal of Waste2Taste is to reduce avoidable food waste by helping users participate in a rescue and reuse flow that brings meals closer to people who need them while respecting the food supplier experience.
