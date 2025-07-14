

- Swift
- Duration
- Duration.TimeFormatStyle
-  attributed 

Instance Property

# attributed

A property that formats the duration as an attributed string.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var attributed: Duration.TimeFormatStyle.Attributed { get }
```

## Discussion

Apply the `attributed` property to a configured Duration.TimeFormatStyle to produce an Duration.TimeFormatStyle.Attributed style. You can then format a duration with this style to create a formatted AttributedString. The formatted attributed string contains instances of AttributeScopes.FoundationAttributes.DateFieldAttribute for runs with formatted durations.

The following example formats a duration as an attributed string:

```
let duration = Duration.seconds(70 * 60 + 32) +
    Duration.milliseconds(400)
let style = Duration.TimeFormatStyle(pattern: .hourMinuteSecond).attributed
let attributedDuration = duration.formatted(style)
```

The resulting `attributedDuration`, representing the string `1:10:32` contains the following runs:

| Run  | Attributes                                     |
|------|------------------------------------------------|
| `1`  | `Foundation.DurationFormatAttribute = hours`   |
| `:`  | None                                           |
| `10` | `Foundation.DurationFormatAttribute = minutes` |
| `:`  | None                                           |
| `32` | `Foundation.DurationFormatAttribute = seconds` |

## See Also

### Formatting a duration as an attributed string

struct Attributed

A format style that formats durations as attributed strings.

