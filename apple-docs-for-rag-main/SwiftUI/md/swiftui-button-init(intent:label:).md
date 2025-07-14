

- SwiftUI
- Button
-  init(intent:label:) 

Initializer

# init(intent:label:)

Creates a button that performs an `AppIntent`.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
init(
    intent: I,
    @ViewBuilder label: () -> Label
) where I : AppIntent
```

Available when `Label` conforms to `View`.

## Parameters 

`intent`  

The `AppIntent` to execute.

`label`  

A view that describes the purpose of the button’s `action`.

## See Also

### Creating a button to perform an App Intent

init(_:intent:)

Creates a button that performs an `AppIntent` and generates its label from a localized string key.

init(_:role:intent:)

Creates a button with a specified role that performs an `AppIntent` and generates its label from a string.

init(role: ButtonRole?, intent: some AppIntent, label: () -> Label)

Creates a button with a specified role that performs an `AppIntent`.

init(_:image:role:intent:)

Creates a button with a specified role that generates its label from a string and an image resource.

init(_:systemImage:role:intent:)

Creates a button with a specified role that generates its label from a string and a system image.

