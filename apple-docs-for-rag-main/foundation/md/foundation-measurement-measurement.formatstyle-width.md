

- Foundation
- Measurement
- Measurement.FormatStyle
-  width 

Instance Property

# width

The width of the measurement unit.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var width: Measurement.FormatStyle.UnitWidth
```

## Discussion

The `width` property specifies the display of the measurement unit. The possible values are abbreviated, narrow, and wide. The format style represents the unit in the shortest notation available.

The following example shows *100 degrees Fahrenheit* in each width for the `en_US` locale.

```
let temperatureMeasurement = Measurement(value: 100, unit: .fahrenheit)
temperatureMeasurement.formatted(.measurement(width: .wide)) // 100 degrees Fahrenheit
temperatureMeasurement.formatted(.measurement(width: .abbreviated)) // 100°F
temperatureMeasurement.formatted(.measurement(width: .narrow)) // 100°
```

## See Also

### Modifying a measurement format style

struct UnitWidth

Specifies the width of the unit, determining the textual representation.

var numberFormatStyle: FloatingPointFormatStyle&lt;Double>?

The formatting of the measurement value.

var usage: MeasurementFormatUnitUsage&lt;UnitType>?

The intended purpose of the formatted measurement.

var hidesScaleName: Bool

The visibility of the unit name of a temperature.

var locale: Locale

The locale of the format style.

