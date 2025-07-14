

- SwiftUI
-  AppStorage 

Structure

# AppStorage

A property wrapper type that reflects a value from `UserDefaults` and invalidates a view on a change in value in that user default.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen @propertyWrapper
struct AppStorage
```

## Topics

### Storing a value

init(wrappedValue:_:store:)

Creates a property that can save and restore tab sidebar customizations.

init(_:store:)

Creates a property that can read and write an Optional boolean user default.

### Getting the value

var wrappedValue: Value

var projectedValue: Binding&lt;Value>

## Relationships

### Conforms To

- DynamicProperty
- Sendable

## See Also

### Saving state across app launches

Restoring Your App’s State with SwiftUI

Provide app continuity for users by preserving their current activities.

func defaultAppStorage(UserDefaults) -> some View

The default store used by `AppStorage` contained within the view.

struct SceneStorage

A property wrapper type that reads and writes to persisted, per-scene storage.

