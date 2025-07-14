

- Foundation
- MeasurementFormatter
-  unitStyle 

Instance Property

# unitStyle

The unit style.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var unitStyle: Formatter.UnitStyle { get set }
```

## Discussion

The possible values are Formatter.UnitStyle.short, Formatter.UnitStyle.medium, and Formatter.UnitStyle.long. The default value is Formatter.UnitStyle.medium.

## See Also

### Specifying the Format

var unitOptions: MeasurementFormatter.UnitOptions

The options for how the unit is formatted.

var locale: Locale!

The locale of the formatter.

var numberFormatter: NumberFormatter!

The number formatter used to format the quantity of a measurement.

