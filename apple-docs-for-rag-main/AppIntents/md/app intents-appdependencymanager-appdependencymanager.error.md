

- App Intents
- AppDependencyManager
-  AppDependencyManager.Error 

Enumeration

# AppDependencyManager.Error

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
enum Error
```

## Topics

### Enumeration Cases

case failedToLoadDependency(AnyHashable, Value.Type)

case failedToRetrieveDependency(AnyHashable, Value.Type)

case incorrectDependencyType(AnyHashable, Value.Type, any Any.Type)

### Instance Properties

var errorDescription: String?

A localized message describing what error occurred.

### Default Implementations

Error Implementations

LocalizedError Implementations

## Relationships

### Conforms To

- Error
- LocalizedError
- Sendable

