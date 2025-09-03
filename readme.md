# Library App

## Recent Changes & Achievements

- Refactored solution for improved modularity and separation of concerns.
- Enhanced test coverage for core entities and services.
- Added support for configuration via `appSettings.json` and JSON data files.
- Improved console UI for better user experience.
- Implemented clean architecture principles across all layers.
- Added new domain entities and extended business logic in services.
- Streamlined build and run instructions for easier onboarding.

## Description

Library App is a modular .NET solution for managing library operations, including books, authors, patrons, and loans. It is designed with clean architecture principles, separating core logic, infrastructure, and console interface for maintainability and extensibility.

## Project Structure

- GuidedProjectApp.sln
- AccelerateDevGitHubCopilot/
  - readme.md
  - src/
    - Library.ApplicationCore/
      - Library.ApplicationCore.csproj
      - Entities/
      - Enums/
      - Interfaces/
      - Services/
    - Library.Console/
      - appSettings.json
      - CommonActions.cs
      - ConsoleApp.cs
      - ConsoleState.cs
      - Library.Console.csproj
      - Program.cs
      - Json/
    - Library.Infrastructure/
      - Library.Infrastructure.csproj
      - (other infrastructure files)
  - tests/
    - UnitTests/
      - (unit test files)

## Key Classes and Interfaces

- **Entities**
  - Represents core domain models such as Book, Author, Patron, Loan.
- **Enums**
  - Defines enumerations for statuses and types used throughout the app.
- **Interfaces**
  - Abstractions for services and repositories, e.g., `IBookService`, `IPatronRepository`.
- **Services**
  - Business logic implementations for library operations.
- **ConsoleApp**
  - Entry point for the console interface, handling user interaction.
- **CommonActions**
  - Shared actions and utilities for the console UI.
- **ConsoleState**
  - Maintains state for the console session.

## Usage

1. **Build the Solution**
   - Open the solution in Visual Studio or VS Code.
   - Run the following command in the root directory:
     ```sh
     dotnet build
     ```

2. **Run the Console Application**
   - Navigate to the `src/Library.Console` directory.
   - Execute:
     ```sh
     dotnet run
     ```

3. **Configuration**
   - Edit `appSettings.json` and files in `Json/` to customize initial data and settings.

4. **Testing**
   - Run unit tests from the `tests/UnitTests` directory:
     ```sh
     dotnet test
     ```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file
