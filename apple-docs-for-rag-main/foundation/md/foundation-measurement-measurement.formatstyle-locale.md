

- Foundation
- Measurement
- Measurement.FormatStyle
-  locale 

Instance Property

# locale

The locale of the format style.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var locale: Locale
```

## Discussion

By default, the format style displays a measurement in the unit that `locale` specifies. The default value is autoupdatingCurrent.

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

var hidesScaleName: Bool

The visibility of the unit name of a temperature.

