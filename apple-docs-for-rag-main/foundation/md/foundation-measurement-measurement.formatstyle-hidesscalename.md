

- Foundation
- Measurement
- Measurement.FormatStyle
-  hidesScaleName 

Instance Property

# hidesScaleName

The visibility of the unit name of a temperature.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var hidesScaleName: Bool { get set }
```

Available when `UnitType` is `UnitTemperature`.

## Discussion

Set `hidesScaleName` to `true` to exclude the unit name from a formatted temperature string. For example, `90°` rather than `90°F` or `90°C` with the narrow unit width, or `90 degrees` rather than `90 degrees Celcius` or `90 degrees Fahrenheit` with the wide width.

Hiding the unit name only affects the presentation of the measurement. Unless you specify `asProvided` as the `usage`, the system converts the temperature to the unit that the locale uses.

## See Also

### Modifying a measurement format style

var width: Measurement&lt;UnitType>.FormatStyle.UnitWidth

The width of the measurement unit.

struct UnitWidth

Specifies the width of the unit, determining the textual representation.

var numberFormatStyle: FloatingPointFormatStyle&lt;Double>?

The formatting of the measurement value.

var usage: MeasurementFormatUnitUsage&lt;UnitType>?

The intended purpose of the formatted measurement.

var locale: Locale

The locale of the format style.

