

- Swift
- Duration
- Duration.TimeFormatStyle
-  Duration.TimeFormatStyle.Attributed 

Structure

# Duration.TimeFormatStyle.Attributed

A format style that formats durations as attributed strings.

SwiftFoundationiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@dynamicMemberLookup
struct Attributed
```

## Overview

Apply the Duration.TimeFormatStyle.Attributed property to a configured Duration.TimeFormatStyle to produce an instance of this style. You can then format a duration with this style to create a formatted AttributedString. The formatted attributed string contains instances of AttributeScopes.FoundationAttributes.DateFieldAttribute for runs with formatted durations.

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

## Topics

### Formatting a duration

func format(Duration) -> AttributedString

Creates a locale-aware attributed string representation from a duration value.

### Working with locales

func locale(Locale) -> Duration.TimeFormatStyle.Attributed

Modifies the format style to use the specified locale.

### Instance Methods

func grouping(NumberFormatStyleConfiguration.Grouping) -> Duration.TimeFormatStyle.Attributed

Returns a modified style that applies the given `grouping` rule to the highest field in the pattern.

### Subscripts

subscript&lt;T>(dynamicMember _: WritableKeyPath&lt;Duration.TimeFormatStyle, T>) -> T

subscript&lt;T>(dynamicMember _: KeyPath&lt;Duration.TimeFormatStyle, T>) -> T

## Relationships

### Conforms To

- Copyable
- Decodable
- DiscreteFormatStyle
- Encodable
- Equatable
- FormatStyle
- Hashable
- Sendable

## See Also

### Formatting a duration as an attributed string

var attributed: Duration.TimeFormatStyle.Attributed

A property that formats the duration as an attributed string.

