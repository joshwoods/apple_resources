

- Foundation
- Measurement
- Measurement.FormatStyle
-  usage 

Instance Property

# usage

The intended purpose of the formatted measurement.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var usage: MeasurementFormatUnitUsage?
```

## Discussion

You can use the `usage` property to specify the intended purpose of the formatted measurement. The default option, `general`, formats the measurement with the default unit for the current locale. The `asProvided` option formats the measurement using the specified unit, ignoring the unit that the locale uses.

The following example shows a formatted temperature using the default unit for the `en_US` locale and using a provided Celsius unit:

```
let temperature = Measurement(value: 36.8, unit: .celsius)
temperature.formatted()
// 98°F

temperature.formatted(.measurement(width: .abbreviated, usage: .asProvided))
// 36.8°C
```

All unit types have `general` and `asProvided` options. Some subclasses have additional options, such as the following:

UnitTemperature

- `person`

- `weather`

UnitLength

- `person`

- `personHeight`

- `road`

UnitEnergy

- `food`

- `workout`

UnitMass

- `personWeight`

## See Also

### Modifying a measurement format style

var width: Measurement&lt;UnitType>.FormatStyle.UnitWidth

The width of the measurement unit.

struct UnitWidth

Specifies the width of the unit, determining the textual representation.

var numberFormatStyle: FloatingPointFormatStyle&lt;Double>?

The formatting of the measurement value.

var hidesScaleName: Bool

The visibility of the unit name of a temperature.

var locale: Locale

The locale of the format style.

