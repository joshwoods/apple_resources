

- ClockKit
- CLKSimpleTextProvider
-  shortText Deprecated

Instance Property

# shortText

A shorter version of the text.

watchOS 2.0–9.0Deprecated

``` source
var shortText: String? { get set }
```

Deprecated

On watchOS 9.0 or later, use WidgetKit instead

## Discussion

The text provider uses this string before attempting to truncate the long version of your text. In this string, you might use abbreviations instead of full words or include only the most important word or characters.

## See Also

### Getting the Text

var text: String

The long version of text that you want to display.

Deprecated

