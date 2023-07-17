# Rick and Morty app

## 1. GitFlow
Branches: main, dev, feature/..., bugfix/...
Commit name structure: Description 

## 2. Architecture
Clean Architecture + BloC
Dependency Injection: GetIt
Domain layer: models, repositories, use-cases.
Data layer: entities, mappers from entities to domain model, implementations of repositories and providers.

## 3. Project structure
Modules: core, core_ui, navigation, data, domain, etc.

## 4. Code Development Rules
Lint rules described in analysis_options.yaml

## 5. Asynchrony support
Flutter Async

## 6. Abstractions for data sources and data access
Providers are responsible for specific services (e.g. http provider, local provider, etc.),
they use data layer entities. Do not have abstract base classes.
Repositories are responsible for gathering data from providers
and mapping it to the corresponding domain layer models. Have abstract base classes in domain layer.

## 7. Approach for working with UI
One file = one widget.
Screen widget contains BlocProviders.

## 8. Localization
Localization is implemented using Localise service.

## 9. Design system
Fonts, colors, frequently used constant values, and icons are stored in core_ui module.

## 10. Supported platforms
Mobiles - iOS and Android