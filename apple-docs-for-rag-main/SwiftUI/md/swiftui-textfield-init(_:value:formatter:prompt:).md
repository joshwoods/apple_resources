

- SwiftUI
- TextField
-  init(\_:value:formatter:prompt:) 

Initializer

# init(\_:value:formatter:prompt:)

Creates a text field that applies a formatter to a bound value, with a label generated from a title string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
init(
    _ title: S,
    value: Binding,
    formatter: Formatter,
    prompt: Text?
) where S : StringProtocol
```

Available when `Label` is `Text`.

Show all declarations

## Parameters 

`title`  

The title of the text field, describing its purpose.

`value`  

The underlying value to edit.

`formatter`  

A formatter to use when converting between the string the user edits and the underlying value of type `V`. If `formatter` can’t perform the conversion, the text field doesn’t modify `binding.value`.

`prompt`  

A `Text` which provides users with guidance on what to enter into the text field.

## Discussion

Use this initializer to create a text field that binds to a bound value, using a Formatter to convert to and from this type. Changes to the bound value update the string displayed by the text field. Editing the text field updates the bound value, as long as the formatter can parse the text. If the format style can’t parse the input, the bound value remains unchanged.

Use the onSubmit(of:_:) modifier to invoke an action whenever the user submits this text field.

The following example uses a Double as the bound value, and a NumberFormatter instance to convert to and from a string representation. The formatter uses the NumberFormatter.Style.decimal style, to allow entering a fractional part. As the user types, the bound value updates, which in turn updates three Text views that use different format styles. If the user enters text that doesn’t represent a valid `Double`, the bound value doesn’t update.

```
@State private var label = "Double"
@State private var myDouble: Double = 0.673
@State private var numberFormatter: NumberFormatter = {
    var nf = NumberFormatter()
    nf.numberStyle = .decimal
    return nf
}()

var body: some View {
    VStack {
        TextField(
            label,
            value: $myDouble,
            formatter: numberFormatter
        )
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

init(value:format:prompt:label:)

Creates a text field that applies a format style to a bound value, with a label generated from a view builder.

init(_:value:formatter:)

Create an instance which binds over an arbitrary type, `V`.

init&lt;V>(value: Binding&lt;V>, formatter: Formatter, prompt: Text?, label: () -> Label)

Creates a text field that applies a formatter to a bound optional value, with a label generated from a view builder.

