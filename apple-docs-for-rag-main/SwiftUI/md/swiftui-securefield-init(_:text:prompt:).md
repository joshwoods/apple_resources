

- SwiftUI
- SecureField
-  init(\_:text:prompt:) 

Initializer

# init(\_:text:prompt:)

Creates a secure field with a prompt generated from a `Text`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    text: Binding,
    prompt: Text?
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the field’s localized title. The title describes the purpose of the field.

`text`  

A binding to the text that the field displays and edits.

`prompt`  

A Text view that represents the secure field’s prompt. The prompt provides guidance on what people should type into the secure field.

## Discussion

Use the onSubmit(of:_:) modifier to invoke an action whenever someone submits this secure field — for example, by pressing the Return key.

## See Also

### Creating a secure text field

init(_:text:)

Creates a secure field with a prompt generated from a `Text`.

init(text: Binding&lt;String>, prompt: Text?, label: () -> Label)

Creates a secure field with a prompt generated from a `Text`.

