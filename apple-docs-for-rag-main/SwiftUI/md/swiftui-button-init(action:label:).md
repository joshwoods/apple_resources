

- SwiftUI
- Button
-  init(action:label:) 

Initializer

# init(action:label:)

Creates a button that displays a custom label.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@preconcurrency
init(
    action: @escaping @MainActor () -> Void,
    @ViewBuilder label: () -> Label
)
```

## Parameters 

`action`  

The action to perform when the user triggers the button.

`label`  

A view that describes the purpose of the button’s `action`.

## See Also

### Creating a button

init(_:action:)

Creates a button that generates its label from a localized string key.

init(_:image:action:)

Creates a button that generates its label from a localized string key and image resource.

init(_:systemImage:action:)

Creates a button that generates its label from a localized string key and system image name.

