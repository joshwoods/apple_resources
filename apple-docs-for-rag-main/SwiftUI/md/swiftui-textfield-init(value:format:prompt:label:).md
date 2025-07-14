

- SwiftUI
- TextField
-  init(value:format:prompt:label:) 

Initializer

# init(value:format:prompt:label:)

Creates a text field that applies a format style to a bound value, with a label generated from a view builder.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
init(
    value: Binding,
    format: F,
    prompt: Text? = nil,
    @ViewBuilder label: () -> Label
) where F : ParseableFormatStyle, F.FormatOutput == String
```

Available when `Label` conforms to `View`.

Show all declarations

## Parameters 

`value`  

The underlying value to edit.

`format`  

A format style of type `F` to use when converting between the string the user edits and the underlying value of type `F.FormatInput`. If `format` can’t perform the conversion, the text field leaves the value unchanged. If the user stops editing the text in an invalid state, the text field updates the field’s text to the last known valid value.

`prompt`  

A `Text` which provides users with guidance on what to type into the text field.

`label`  

A view builder that produces a label for the text field, describing its purpose.

## Discussion

Use this initializer to create a text field that binds to a bound value, using a ParseableFormatStyle to convert to and from this type. Changes to the bound value update the string displayed by the text field. Editing the text field updates the bound value, as long as the format style can parse the text. If the format style can’t parse the input, the bound value remains unchanged.

Use the onSubmit(of:_:) modifier to invoke an action whenever the user submits this text field.

The following example uses a Double as the bound value, and a FloatingPointFormatStyle instance to convert to and from a string representation. As the user types, the bound value updates, which in turn updates three Text views that use different format styles. If the user enters text that doesn’t represent a valid `Double`, the bound value doesn’t update.

```
@State private var myDouble: Double = 0.673
var body: some View {
    VStack {
        TextField(
            value: $myDouble,
            format: .number
        ) {
            Text("Double")
        }
        Text(myDouble, format: .number)
        Text(myDouble, format: .number.precision(.significantDigits(5)))
        Text(myDouble, format: .number.notation(.scientific))
    }
}
```

## See Also

### Creating a text field with a value

init(_:value:format:prompt:)

Creates a text field that applies a format style to a bound value, with a label generated from a localized title string.

init(_:value:formatter:)

Create an instance which binds over an arbitrary type, `V`.

init(_:value:formatter:prompt:)

Creates a text field that applies a formatter to a bound value, with a label generated from a title string.

init&lt;V>(value: Binding&lt;V>, formatter: Formatter, prompt: Text?, label: () -> Label)

Creates a text field that applies a formatter to a bound optional value, with a label generated from a view builder.

