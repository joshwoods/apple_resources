

- ClockKit
- CLKTextProvider
-  init(format:\_:) Deprecated

Initializer

# init(format:\_:)

Creates and returns a text provider built from the specified format string.

watchOS 6.0–9.0Deprecated

``` source
convenience init(
    format: String,
    _ args: any CVarArg...
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`format`  

A format string to use when building the text provider. To insert content from another text provider into the string, use the `%@` placeholder. For more information and examples about the placeholders you can use in this string, see Formatting String Objects and String Format Specifiers. This parameter must not be `nil`.

`args`  

A comma-separated list of arguments to substitute into `format`.

## Return Value

A text provider object built from the specified arguments.

## Discussion

Use this method to create a text provider comprising text and the content of other objects, including other text providers.

