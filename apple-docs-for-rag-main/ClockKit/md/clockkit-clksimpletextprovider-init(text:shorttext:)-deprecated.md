

- ClockKit
- CLKSimpleTextProvider
-  init(text:shortText:) Deprecated

Initializer

# init(text:shortText:)

Creates and returns a text provider with both long and short versions of the text.

watchOS 2.0–9.0Deprecated

``` source
convenience init(
    text: String,
    shortText: String?
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`text`  

The text that you want to display. This value is assigned to the text property of your text provider object.

`shortText`  

A shorter version of the value in the `text` parameter that conveys the same information.

## Return Value

A text provider initialized with the specified content.

## See Also

### Creating a Text Provider

convenience init(text: String)

Creates and returns a text provider with the specified long form text.

Deprecated

convenience init(text: String, shortText: String?, accessibilityLabel: String?)

Creates and returns a text provider with the text strings and an accessible string.

Deprecated

