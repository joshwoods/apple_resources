

- SwiftUI
- SecureField
-  init(text:prompt:label:) 

Initializer

# init(text:prompt:label:)

Creates a secure field with a prompt generated from a `Text`.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
init(
    text: Binding,
    prompt: Text? = nil,
    @ViewBuilder label: () -> Label
)
```

Available when `Label` conforms to `View`.

## Parameters 

`text`  

A binding to the text that the field displays and edits.

`prompt`  

A Text view that represents the secure field’s prompt. The prompt provides guidance on what people should type into the secure field.

`label`  

A view that describes the purpose of the secure field.

## Discussion

Use the onSubmit(of:_:) modifier to invoke an action whenever someone submits this secure field — for example, by pressing the Return key.

## See Also

### Creating a secure text field

init(_:text:)

Creates a secure field with a prompt generated from a `Text`.

init(_:text:prompt:)

Creates a secure field with a prompt generated from a `Text`.

