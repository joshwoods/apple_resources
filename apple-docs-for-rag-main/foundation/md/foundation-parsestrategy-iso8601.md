

- Foundation
- ParseStrategy
-  iso8601 

Type Property

# iso8601

A style for formatting a date in accordance with the ISO-8601 standard.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var iso8601: Date.ISO8601FormatStyle { get }
```

Available when `Self` is `Date.ISO8601FormatStyle`.

## Discussion

Use the dot-notation form of this type property when the call point allows the use of Date.ISO8601FormatStyle; in other words, when the value type is `Date`. Typically, you use this with the formatted(_:) method of `Date`.

## See Also

### Commonly-used format styles

static var dateTime: Date.FormatStyle

A default format style for formatting dates.

