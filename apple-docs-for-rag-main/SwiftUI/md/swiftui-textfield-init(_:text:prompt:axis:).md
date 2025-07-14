

- SwiftUI
- TextField
-  init(\_:text:prompt:axis:) 

Initializer

# init(\_:text:prompt:axis:)

Creates a text field with a preferred axis and a text label generated from a localized title string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    text: Binding,
    prompt: Text?,
    axis: Axis
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized title of the text field, describing its purpose.

`text`  

The text to display and edit.

`prompt`  

A `Text` representing the prompt of the text field which provides users with guidance on what to type into the text field.

`axis`  

The axis in which to scroll text when it doesn’t fit in the available space.

## Discussion

Specify a preferred axis in which the text field should scroll its content when it does not fit in the available space. Depending on the style of the field, this axis may not be respected.

Use the onSubmit(of:_:) modifier to invoke an action whenever the user submits this text field.

## See Also

### Creating a scrollable text field

init(_:text:axis:)

Creates a text field with a preferred axis and a text label generated from a localized title string.

init(text: Binding&lt;String>, prompt: Text?, axis: Axis, label: () -> Label)

Creates a text field with a preferred axis and a prompt generated from a `Text`.

