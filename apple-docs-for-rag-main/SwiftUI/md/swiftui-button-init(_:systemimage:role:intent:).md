

- SwiftUI
- Button
-  init(\_:systemImage:role:intent:) 

Initializer

# init(\_:systemImage:role:intent:)

Creates a button with a specified role that generates its label from a string and a system image.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
init(
    _ title: some StringProtocol,
    systemImage: String,
    role: ButtonRole? = nil,
    intent: some AppIntent
)
```

Available when `Label` is `Label`.

Show all declarations

## Parameters 

`title`  

A string that describes the purpose of the button’s `intent`.

`systemImage`  

The name of the image resource to lookup.

`role`  

An optional semantic role describing the button. A value of `nil` means that the button doesn’t have an assigned role.

`intent`  

The `AppIntent` to execute.

## Discussion

This initializer creates a Label view on your behalf, and treats the title similar to init(_:). See Text for more information about localizing strings.

## See Also

### Creating a button to perform an App Intent

init(_:intent:)

Creates a button that performs an `AppIntent` and generates its label from a localized string key.

init&lt;I>(intent: I, label: () -> Label)

Creates a button that performs an `AppIntent`.

init(_:role:intent:)

Creates a button with a specified role that performs an `AppIntent` and generates its label from a string.

init(role: ButtonRole?, intent: some AppIntent, label: () -> Label)

Creates a button with a specified role that performs an `AppIntent`.

init(_:image:role:intent:)

Creates a button with a specified role that generates its label from a string and an image resource.

