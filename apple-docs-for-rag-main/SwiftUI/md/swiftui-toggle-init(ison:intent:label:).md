

- SwiftUI
- Toggle
-  init(isOn:intent:label:) 

Initializer

# init(isOn:intent:label:)

Creates a toggle performing an `AppIntent`.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
init(
    isOn: Bool,
    intent: I,
    @ViewBuilder label: () -> Label
) where I : AppIntent
```

Available when `Label` conforms to `View`.

## Parameters 

`isOn`  

Whether the toggle is on or off.

`intent`  

The `AppIntent` to be performed.

`label`  

A view that describes the purpose of the toggle.

## See Also

### Creating a toggle for an App Intent

init(_:isOn:intent:)

Creates a toggle performing an `AppIntent` and generates its label from a localized string key.

