

- SwiftUI
- Toggle
-  init(isOn:label:) 

Initializer

# init(isOn:label:)

Creates a toggle that displays a custom label.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
init(
    isOn: Binding,
    @ViewBuilder label: () -> Label
)
```

## Parameters 

`isOn`  

A binding to a property that determines whether the toggle is on or off.

`label`  

A view that describes the purpose of the toggle.

## See Also

### Creating a toggle

init(_:isOn:)

Creates a toggle that generates its label from a localized string key.

init(_:image:isOn:)

Creates a toggle that generates its label from a localized string key and image resource.

init(_:systemImage:isOn:)

Creates a toggle that generates its label from a localized string key and system image.

