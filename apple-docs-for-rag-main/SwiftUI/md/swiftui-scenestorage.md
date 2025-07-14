

- SwiftUI
-  SceneStorage 

Structure

# SceneStorage

A property wrapper type that reads and writes to persisted, per-scene storage.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@frozen @propertyWrapper
struct SceneStorage
```

## Overview

You use `SceneStorage` when you need automatic state restoration of the value. `SceneStorage` works very similar to `State`, except its initial value is restored by the system if it was previously saved, and the value is shared with other `SceneStorage` variables in the same scene.

The system manages the saving and restoring of `SceneStorage` on your behalf. The underlying data that backs `SceneStorage` is not available to you, so you must access it via the `SceneStorage` property wrapper. The system makes no guarantees as to when and how often the data will be persisted.

Each `Scene` has its own notion of `SceneStorage`, so data is not shared between scenes.

Ensure that the data you use with `SceneStorage` is lightweight. Data of a large size, such as model data, should not be stored in `SceneStorage`, as poor performance may result.

If the `Scene` is explicitly destroyed (e.g. the switcher snapshot is destroyed on iPadOS or the window is closed on macOS), the data is also destroyed. Do not use `SceneStorage` with sensitive data.

## Topics

### Storing a value

init(wrappedValue:_:)

Creates a property that can save and restore an integer, transforming it to a `RawRepresentable` data type.

init(_:)

Creates a property that can save and restore an Optional boolean.

### Getting the value

var wrappedValue: Value

The underlying value referenced by the state variable.

var projectedValue: Binding&lt;Value>

A binding to the state value.

### Initializers

init(wrappedValue: Value, String, store: UserDefaults?)

Creates a property that can save and restore tab sidebar customizations.

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

struct AppStorage

A property wrapper type that reflects a value from `UserDefaults` and invalidates a view on a change in value in that user default.

