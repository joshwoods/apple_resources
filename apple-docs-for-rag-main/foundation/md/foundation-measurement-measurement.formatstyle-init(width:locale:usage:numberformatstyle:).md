

- Foundation
- Measurement
- Measurement.FormatStyle
-  init(width:locale:usage:numberFormatStyle:) 

Initializer

# init(width:locale:usage:numberFormatStyle:)

Creates an instance using the provided width, locale, usage type, and number format.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    width: Measurement.FormatStyle.UnitWidth,
    locale: Locale = .autoupdatingCurrent,
    usage: MeasurementFormatUnitUsage = .general,
    numberFormatStyle: FloatingPointFormatStyle? = nil
)
```

## Parameters 

`width`  

The width of the measurement unit.

`locale`  

The locale to use when formatting the measurement.

`usage`  

The intended purpose of the formatted measurement.

`numberFormatStyle`  

The presentation style of the numeric value.

## See Also

### Creating a measurement format style

init(width: Measurement&lt;UnitType>.FormatStyle.UnitWidth, locale: Locale, usage: MeasurementFormatUnitUsage&lt;UnitType>, hidesScaleName: Bool, numberFormatStyle: FloatingPointFormatStyle&lt;Double>?)

Creates an instance using the provided width, locale, usage type, number format, and the option to hide the unit name.

