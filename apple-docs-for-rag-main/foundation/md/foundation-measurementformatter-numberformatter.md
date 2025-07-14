

- Foundation
- MeasurementFormatter
-  numberFormatter 

Instance Property

# numberFormatter

The number formatter used to format the quantity of a measurement.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var numberFormatter: NumberFormatter! { get set }
```

## Discussion

If unspecified, an NumberFormatter object with NumberFormatter.Style.decimal style is used.

## See Also

### Specifying the Format

var unitOptions: MeasurementFormatter.UnitOptions

The options for how the unit is formatted.

var unitStyle: Formatter.UnitStyle

The unit style.

var locale: Locale!

The locale of the formatter.

