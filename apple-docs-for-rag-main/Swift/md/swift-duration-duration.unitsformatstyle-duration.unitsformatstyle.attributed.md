

- Swift
- Duration
- Duration.UnitsFormatStyle
-  Duration.UnitsFormatStyle.Attributed 

Structure

# Duration.UnitsFormatStyle.Attributed

A format style that formats durations as attributed strings.

SwiftFoundationiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@dynamicMemberLookup
struct Attributed
```

## Overview

Apply the attributed property to a configured Duration.UnitsFormatStyle to produce an instance of this style. You can then format a duration with this style to create a formatted AttributedString. The formatted attributed string contains instances of AttributeScopes.FoundationAttributes.DateFieldAttribute and AttributeScopes.FoundationAttributes.MeasurementAttribute for runs with formatted durations.

The following example formats a duration as an attributed string:

```
let duration = Duration.seconds(70 * 60 + 32) +
    Duration.milliseconds(400)
let style = Duration.UnitsFormatStyle(allowedUnits: [.hours, .minutes, .seconds],
                                      width: .abbreviated).attributed
let attributedDuration = duration.formatted(style)
```

The resulting `attributedDuration`, representing the string `1 hr, 10 min, 32 sec` contains the following runs:

| Run | Attributes |
|----|----|
| `1` | `Foundation.MeasurementAttribute = value`, `Foundation.DurationFormatAttribute = hours` |
| (space) | `Foundation.DurationFormatAttribute = hours` |
| `hr` | `Foundation.DurationFormatAttribute = hours`, `Foundation.MeasurementAttribute = unit` |
| `, ` | None |
| `10` | `Foundation.MeasurementAttribute = value`, `Foundation.DurationFormatAttribute = minutes` |
| (space) | `Foundation.DurationFormatAttribute = minutes` |
| `min` | `Foundation.DurationFormatAttribute = minutes`, `Foundation.MeasurementAttribute = unit` |
| `, ` | None |
| `32` | `Foundation.MeasurementAttribute = value`, `Foundation.DurationFormatAttribute = seconds` |
| (space) | `Foundation.DurationFormatAttribute = seconds` |
| `sec` | `Foundation.DurationFormatAttribute = seconds`, `Foundation.MeasurementAttribute = unit` |

## Topics

### Formatting a duration

func format(Duration) -> AttributedString

Creates a locale-aware attributed string representation from a duration value.

### Working with locales

func locale(Locale) -> Duration.UnitsFormatStyle.Attributed

Modifies the format style to use the specified locale.

### Subscripts

subscript&lt;T>(dynamicMember _: KeyPath&lt;Duration.UnitsFormatStyle, T>) -> T

subscript&lt;T>(dynamicMember _: WritableKeyPath&lt;Duration.UnitsFormatStyle, T>) -> T

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

var attributed: Duration.UnitsFormatStyle.Attributed

A property that formats the duration as an attributed string.

