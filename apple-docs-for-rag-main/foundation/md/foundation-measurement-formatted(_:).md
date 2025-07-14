

- Foundation
- Measurement
-  formatted(\_:) 

Instance Method

# formatted(\_:)

Generates a locale-aware string representation of a measurement using the provided measurement format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func formatted(_ style: S) -> S.FormatOutput where S : FormatStyle, S.FormatInput == Measurement
```

Available when `UnitType` inherits `Dimension`.

## Parameters 

`style`  

The measurement format style to apply to the measurement.

## Return Value

A string, formatted according to the provided style.

## Discussion

Use the formatted(_:) method to create a string representation of a measurement using a custom measurement format style. You can specify the width of the unit name, the numeric formatting of the value, and the intended usage type of the measurement. You can use the Measurement.FormatStyle static factory method `measurement(width:usage:numberFormat:)` to create a custom format style as a parameter to the method, such as in the following example:

```
let temp = Measurement(value: 38, unit: .celsius)
let formattedTemp = temp.formatted(.measurement(width: .wide, usage: .weather, numberFormat: .numeric(precision: .fractionLength(1))))
// For locale: en_US: 100.4 degrees Fahrenheit
```

## See Also

### Formatting a Measurement

func formatted() -> String

Generates a locale-aware string representation of a measurement using the default measurement format style.

struct FormatStyle

A type that provides localized representations of measurements.

struct AttributedStyle

A type that provides localized representations of measurements with an attributed string.

