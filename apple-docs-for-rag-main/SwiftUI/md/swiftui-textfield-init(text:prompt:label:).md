

- SwiftUI
- TextField
-  init(text:prompt:label:) 

Initializer

# init(text:prompt:label:)

Creates a text field with a prompt generated from a `Text`.

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

The text to display and edit.

`prompt`  

A `Text` representing the prompt of the text field which provides users with guidance on what to type into the text field.

`label`  

A view that describes the purpose of the text field.

## Discussion

Use the onSubmit(of:_:) modifier to invoke an action whenever the user submits this text field.

## See Also

### Creating a text field with a string

init(_:text:)

Creates a text field with a text label generated from a localized title string.

init(_:text:prompt:)

Creates a text field with a text label generated from a localized title string.

