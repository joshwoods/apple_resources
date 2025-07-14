

- SwiftUI
- TextField
-  init(\_:text:) 

Initializer

# init(\_:text:)

Creates a text field with a text label generated from a localized title string.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    text: Binding
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized title of the text field, describing its purpose.

`text`  

The text to display and edit.

## See Also

### Creating a text field with a string

init(_:text:prompt:)

Creates a text field with a text label generated from a localized title string.

init(text: Binding&lt;String>, prompt: Text?, label: () -> Label)

Creates a text field with a prompt generated from a `Text`.

