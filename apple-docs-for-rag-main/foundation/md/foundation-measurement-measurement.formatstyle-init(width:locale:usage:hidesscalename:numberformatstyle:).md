

- Foundation
- Measurement
- Measurement.FormatStyle
-  init(width:locale:usage:hidesScaleName:numberFormatStyle:) 

Initializer

# init(width:locale:usage:hidesScaleName:numberFormatStyle:)

Creates an instance using the provided width, locale, usage type, number format, and the option to hide the unit name.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
init(
    width: Measurement.FormatStyle.UnitWidth = .abbreviated,
    locale: Locale = .autoupdatingCurrent,
    usage: MeasurementFormatUnitUsage = .general,
    hidesScaleName: Bool = false,
    numberFormatStyle: FloatingPointFormatStyle? = nil
)
```

Available when `UnitType` is `UnitTemperature`.

## Parameters 

`width`  

The width of the measurement unit.

`locale`  

The locale to use when formatting the measurement.

`usage`  

The intended purpose of the formatted measurement.

`hidesScaleName`  

An option to hide the unit name of a measurement.

`numberFormatStyle`  

The presentation style of the numeric value.

## See Also

### Creating a measurement format style

init(width: Measurement&lt;UnitType>.FormatStyle.UnitWidth, locale: Locale, usage: MeasurementFormatUnitUsage&lt;UnitType>, numberFormatStyle: FloatingPointFormatStyle&lt;Double>?)

Creates an instance using the provided width, locale, usage type, and number format.

