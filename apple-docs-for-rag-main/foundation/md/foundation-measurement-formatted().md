

- Foundation
- Measurement
-  formatted() 

Instance Method

# formatted()

Generates a locale-aware string representation of a measurement using the default measurement format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func formatted() -> String
```

Available when `UnitType` inherits `Dimension`.

## Return Value

A string, formatted according to the default style.

## Discussion

Use the formatted() method to apply the default format style to a measurement, such as in the following example:

```
let string = Measurement(value: 38, unit: .celsius).formatted()
// For locale: en_US: 100.4°F
```

The default measurement format style uses an abbreviated unit width, the general usage type, and the default number format style. To customize the formatted measurement string, use the formatted(_:) method and include a Measurement.FormatStyle.

## See Also

### Formatting a Measurement

func formatted&lt;S>(S) -> S.FormatOutput

Generates a locale-aware string representation of a measurement using the provided measurement format style.

struct FormatStyle

A type that provides localized representations of measurements.

struct AttributedStyle

A type that provides localized representations of measurements with an attributed string.

