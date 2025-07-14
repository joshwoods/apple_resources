

- App Intents
-  AppDependencyManager 

Class

# AppDependencyManager

An object that manages the registration and initialization of an app intent’s dependencies.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
final class AppDependencyManager
```

## Mentioned in 

Responding to the Action button on Apple Watch Ultra

## Topics

### Initializers

init()

Can be used to initialize a standalone `AppDependencyManager` for dependency injection during testing.

### Instance Methods

func add&lt;Dependency>(key: AnyHashable?, dependency: @autoclosure () -> () throws -> Dependency)

func add&lt;Dependency>(key: AnyHashable?, dependency: @autoclosure () -> Dependency)

func add&lt;Dependency>(key: AnyHashable?, dependency: () async throws -> Dependency)

### Type Properties

static var shared: AppDependencyManager

### Enumerations

enum Error

## See Also

### Dependency management

class AppDependency

A property wrapper that resolves a registered dependency at runtime.

