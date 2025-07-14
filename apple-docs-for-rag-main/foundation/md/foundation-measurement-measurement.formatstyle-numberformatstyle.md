

- Foundation
- Measurement
- Measurement.FormatStyle
-  numberFormatStyle 

Instance Property

# numberFormatStyle

The formatting of the measurement value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var numberFormatStyle: FloatingPointFormatStyle?
```

## Discussion

The `numberFormat` property specifies the formatting of the measurement value. You can customize the precision, grouping, and rounding mode of the measurement by creating a numeric number format style.

The following example shows a customized measurement format style that includes two decimal numbers and excludes separators:

```
let volume = Measurement(value: 2300, unit: .milliliters)
volume.formatted(.measurement(width: .abbreviated,
                              usage: .asProvided,
                              numberFormatStyle: .number
                                  .precision(.fractionLength(2))
                                  .grouping(.never))) // "2300.00 mL"
```

## See Also

### Modifying a measurement format style

var width: Measurement&lt;UnitType>.FormatStyle.UnitWidth

The width of the measurement unit.

struct UnitWidth

Specifies the width of the unit, determining the textual representation.

var usage: MeasurementFormatUnitUsage&lt;UnitType>?

The intended purpose of the formatted measurement.

var hidesScaleName: Bool

The visibility of the unit name of a temperature.

var locale: Locale

The locale of the format style.

