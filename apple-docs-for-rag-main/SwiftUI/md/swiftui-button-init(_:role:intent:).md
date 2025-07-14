

- SwiftUI
- Button
-  init(\_:role:intent:) 

Initializer

# init(\_:role:intent:)

Creates a button with a specified role that performs an `AppIntent` and generates its label from a string.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
init(
    _ title: some StringProtocol,
    role: ButtonRole?,
    intent: some AppIntent
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`title`  

A string that describes the purpose of the button’s `intent`.

`role`  

An optional semantic role describing the button. A value of `nil` means that the button doesn’t have an assigned role.

`intent`  

The `AppIntent` to execute.

## Discussion

This initializer creates a Text view on your behalf, and treats the title similar to init(_:). See Text for more information about localizing strings.

## See Also

### Creating a button to perform an App Intent

init(_:intent:)

Creates a button that performs an `AppIntent` and generates its label from a localized string key.

init&lt;I>(intent: I, label: () -> Label)

Creates a button that performs an `AppIntent`.

init(role: ButtonRole?, intent: some AppIntent, label: () -> Label)

Creates a button with a specified role that performs an `AppIntent`.

init(_:image:role:intent:)

Creates a button with a specified role that generates its label from a string and an image resource.

init(_:systemImage:role:intent:)

Creates a button with a specified role that generates its label from a string and a system image.

