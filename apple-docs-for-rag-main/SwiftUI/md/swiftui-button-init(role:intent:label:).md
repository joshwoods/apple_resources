

- SwiftUI
- Button
-  init(role:intent:label:) 

Initializer

# init(role:intent:label:)

Creates a button with a specified role that performs an `AppIntent`.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
init(
    role: ButtonRole?,
    intent: some AppIntent,
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View`.

## Parameters 

`role`  

An optional semantic role describing the button. A value of `nil` means that the button doesn’t have an assigned role.

`intent`  

The `AppIntent` to execute.

`label`  

A view that describes the purpose of the button’s `action`.

## See Also

### Creating a button to perform an App Intent

init(_:intent:)

Creates a button that performs an `AppIntent` and generates its label from a localized string key.

init&lt;I>(intent: I, label: () -> Label)

Creates a button that performs an `AppIntent`.

init(_:role:intent:)

Creates a button with a specified role that performs an `AppIntent` and generates its label from a string.

init(_:image:role:intent:)

Creates a button with a specified role that generates its label from a string and an image resource.

init(_:systemImage:role:intent:)

Creates a button with a specified role that generates its label from a string and a system image.

