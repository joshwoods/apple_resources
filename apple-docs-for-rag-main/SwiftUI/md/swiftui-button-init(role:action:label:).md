

- SwiftUI
- Button
-  init(role:action:label:) 

Initializer

# init(role:action:label:)

Creates a button with a specified role that displays a custom label.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@preconcurrency nonisolated
init(
    role: ButtonRole?,
    action: @escaping @MainActor () -> Void,
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View`.

## Parameters 

`role`  

An optional semantic role that describes the button. A value of `nil` means that the button doesn’t have an assigned role.

`action`  

The action to perform when the user interacts with the button.

`label`  

A view that describes the purpose of the button’s `action`.

## See Also

### Creating a button with a role

init(_:role:action:)

Creates a button with a specified role that generates its label from a localized string key.

init(_:image:role:action:)

Creates a button with a specified role that generates its label from a localized string key and an image resource.

init(_:systemImage:role:action:)

Creates a button with a specified role that generates its label from a localized string key and a system image.

