

- SwiftUI
- TextField
-  init(\_:text:selection:prompt:axis:) 

Initializer

# init(\_:text:selection:prompt:axis:)

Creates a text field with a binding to the current selection and a text label generated from a localized title string.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
nonisolated
init(
    _ titleKey: LocalizedStringKey,
    text: Binding,
    selection: Binding,
    prompt: Text? = nil,
    axis: Axis? = nil
)
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`titleKey`  

The key for the localized title of the text field, describing its purpose.

`text`  

The text to display and edit.

`selection`  

A Binding to the variable containing the selection.

`prompt`  

A `Text` representing the prompt of the text field which provides users with guidance on what to type into the text field. Defaults to `nil`.

`axis`  

The axis in which to scroll text when it doesn’t fit in the available space. Defaults to `nil`.

## Discussion

The following example shows a text field with a binding the the current selection:

```
@State private var message: String = ""
@State private var selection: TextSelection? = nil

var body: some View {
    TextField(
        "Message",
        text: $message,
        selection: $selection
    )
}
```

Use the onSubmit(of:_:) modifier to invoke an action whenever the user submits this text field.

