

- App Intents
-  AppDependency 

Class

# AppDependency

A property wrapper that resolves a registered dependency at runtime.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@propertyWrapper
final class AppDependency where Value : Sendable
```

## Mentioned in 

Responding to the Action button on Apple Watch Ultra

## Topics

### Initializers

convenience init(key: AnyHashable?, manager: AppDependencyManager)

convenience init(key: AnyHashable?, manager: AppDependencyManager, default: () async throws -> Value)

convenience init(key: AnyHashable?, manager: AppDependencyManager, default: @autoclosure () -> Value)

### Instance Properties

var projectedValue: AppDependency&lt;Value>

var wrappedValue: Value

## Relationships

### Conforms To

- Sendable

## See Also

### Dependency management

class AppDependencyManager

An object that manages the registration and initialization of an app intent’s dependencies.

