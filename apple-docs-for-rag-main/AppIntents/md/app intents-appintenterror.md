

- App Intents
-  AppIntentError 

Structure

# AppIntentError

Errors that your intent-handling code can return to indicate problems while interpreting or executing an app intent.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct AppIntentError
```

## Topics

### Getting the error codes

static var restartPerform: AppIntentError

### Enumerations

enum PermissionRequired

Errors that indicate that the app doesn’t have required permission to perform an action

enum Unrecoverable

Unknown or unrecoverable error that might have occurred due to either a system or user error.

enum UserActionRequired

Errors that represent a state where a person needs to do respond in order to successfully completed successfully the action.

### Default Implementations

CustomLocalizedStringResourceConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

Error Implementations

## Relationships

### Conforms To

- Copyable
- CustomLocalizedStringResourceConvertible
- CustomStringConvertible
- Equatable
- Error
- Sendable

