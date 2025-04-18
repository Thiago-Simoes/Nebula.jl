# Changelog
## [Unreleased]

### Upcoming
- **More Complex SQL Operations**
  - Support for advanced filters, ordering, and pagination.
- **Security and SQL Injection Prevention**
  - Further input sanitization to complement prepared statements.
- **Transaction Support**
  - Add transaction mechanisms (begin, commit, and rollback) for atomic operations.
- **Connection Pooling**
  - Implement a connection pool to improve performance and prevent database overload.
- **Error Handling and Logging**
  - Improve exception handling and add logs to facilitate debugging.

## [0.2.1]
### Added
- **More Complex SQL Operations**
  - Support for advanced filters, ordering, and pagination.
- **SQL to Julia Type Mapping Expansion**
  - Include support for more types (e.g., DATE, TIMESTAMP, etc.).
## Improved
- **Type Mapping using Macros**
  - Each type can be declared using a macro, instead of a function.
- **Better folders/files organization**
  - Improved readability and maintainability

## [0.2.0]
### Added
- **Relationship between Models**
  - Support for relationships between models, like foreign key.

## [0.1.1] - 2025-02-18
### Added
- **Created a `changelog.md`**
- **Improved Readme and Documentation**
  - Now readme is complete and including license.
  - Implemented documentation using Documenter.jl.

## [0.1.0] - 2025-02-17
### Added
- **Database Connection**
  - Use of environment variables with DotEnv to configure the connection.
- **Table Creation and Migration**
  - `migrate!` function and `@Model` macro that automatically create models and tables.
- **Global Model Registry**
  - Storage of metadata in a global dictionary.
- **Column and Constraint Definitions via Macros**
  - Macros for `@PrimaryKey`, `@AutoIncrement`, `@NotNull`, and `@Unique`.
- **Basic CRUD Operations**
  - Functions for `create`, `update`, `delete`, `findMany`, `findFirst`, `findUnique`, among others.
- **Model Conversion and Instantiation**
  - Conversion of query results into model instances.
- **UUID Generation**
  - `generateUuid` function to create unique identifiers.
- **Prepared Statements**
  - Implemented prepared statements to enhance security and prevent SQL injection.
