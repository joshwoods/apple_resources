

- SwiftUI
- Button
-  init(\_:intent:) 

Initializer

# init(\_:intent:)

Creates a button that performs an `AppIntent` and generates its label from a localized string key.

AppIntentsSwiftUIiOS 17.0+iPadOS 17.0+macOS 14.0+tvOS 17.0+watchOS 10.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    intent: some AppIntent
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the button’s localized title, that describes the purpose of the button’s `intent`.

`intent`  

The `AppIntent` to execute.

## Discussion

This initializer creates a Text view on your behalf, and treats the localized key similar to init(_:tableName:bundle:comment:). See Text for more information about localizing strings.

To initialize a button with a string variable, use init(_:intent:) instead.

## See Also

### Creating a button to perform an App Intent

init&lt;I>(intent: I, label: () -> Label)

Creates a button that performs an `AppIntent`.

init(_:role:intent:)

Creates a button with a specified role that performs an `AppIntent` and generates its label from a string.

init(role: ButtonRole?, intent: some AppIntent, label: () -> Label)

Creates a button with a specified role that performs an `AppIntent`.

init(_:image:role:intent:)

Creates a button with a specified role that generates its label from a string and an image resource.

init(_:systemImage:role:intent:)

Creates a button with a specified role that generates its label from a string and a system image.

