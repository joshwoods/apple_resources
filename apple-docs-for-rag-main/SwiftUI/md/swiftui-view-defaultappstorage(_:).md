

- SwiftUI
- View
-  defaultAppStorage(\_:) 

Instance Method

# defaultAppStorage(\_:)

The default store used by `AppStorage` contained within the view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func defaultAppStorage(_ store: UserDefaults) -> some View
```

## Parameters 

`store`  

The user defaults to use as the default store for `AppStorage`.

## Discussion

If unspecified, the default store for a view hierarchy is `UserDefaults.standard`, but can be set a to a custom one. For example, sharing defaults between an app and an extension can override the default store to one created with `UserDefaults.init(suiteName:_)`.

## See Also

### Saving state across app launches

Restoring Your App’s State with SwiftUI

Provide app continuity for users by preserving their current activities.

struct AppStorage

A property wrapper type that reflects a value from `UserDefaults` and invalidates a view on a change in value in that user default.

struct SceneStorage

A property wrapper type that reads and writes to persisted, per-scene storage.

