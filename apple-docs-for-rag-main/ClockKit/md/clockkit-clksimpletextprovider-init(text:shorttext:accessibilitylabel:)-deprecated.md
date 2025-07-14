

- ClockKit
- CLKSimpleTextProvider
-  init(text:shortText:accessibilityLabel:) Deprecated

Initializer

# init(text:shortText:accessibilityLabel:)

Creates and returns a text provider with the text strings and an accessible string.

watchOS 2.0–9.0Deprecated

``` source
convenience init(
    text: String,
    shortText: String?,
    accessibilityLabel: String?
)
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Parameters 

`text`  

The text that you want to display.

`shortText`  

A shorter version of the value in the `text` parameter that conveys the same information.

`accessibilityLabel`  

A succinct string that identifies the purpose of the text.

## Return Value

A text provider initialized with the specified content.

## See Also

### Creating a Text Provider

convenience init(text: String)

Creates and returns a text provider with the specified long form text.

Deprecated

convenience init(text: String, shortText: String?)

Creates and returns a text provider with both long and short versions of the text.

Deprecated

