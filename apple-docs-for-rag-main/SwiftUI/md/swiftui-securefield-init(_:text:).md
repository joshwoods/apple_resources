

- SwiftUI
- SecureField
-  init(\_:text:) 

Initializer

# init(\_:text:)

Creates a secure field with a prompt generated from a `Text`.

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

The key for the field’s localized title. The title describes the purpose of the field.

`text`  

A binding to the text that the field displays and edits.

## Discussion

Use the onSubmit(of:_:) modifier to invoke an action whenever someone submits this secure field — for example, by pressing the Return key.

## See Also

### Creating a secure text field

init(_:text:prompt:)

Creates a secure field with a prompt generated from a `Text`.

init(text: Binding&lt;String>, prompt: Text?, label: () -> Label)

Creates a secure field with a prompt generated from a `Text`.

