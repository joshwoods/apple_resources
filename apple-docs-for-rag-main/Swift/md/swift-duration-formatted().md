

- Swift
- Duration
-  formatted() 

Instance Method

# formatted()

Formats the string using a localized hour-minute-second time pattern.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func formatted() -> String
```

## Return Value

A localized formatted string that describes the duration, such as `1:30:56` for a duration of 1 hour, 30 minutes, and 56 seconds in the U.S. English locale. In the Finnish locale, this returns `1.30.56`.

## Discussion

The following example shows the effect of applying the default formatting to a duration of two seconds:

```
let duration = Duration.seconds(2)
let formattedDuration = duration.formatted() // "0:00:02"
```

This method uses a default Duration.TimeFormatStyle. To modify the formatting, customize a Duration.TimeFormatStyle or Duration.UnitsFormatStyle, then call formatted(_:) on the duration, passing in the style. You can also call `format(_:)` on the style, passing in a duration.

## See Also

### Formatting a duration

func formatted&lt;S>(S) -> S.FormatOutput

Formats the duration, using the provided format style.

struct TimeFormatStyle

A format style that shows durations in a compact, localized format with separators.

struct UnitsFormatStyle

A format style that shows durations with localized labeled components

