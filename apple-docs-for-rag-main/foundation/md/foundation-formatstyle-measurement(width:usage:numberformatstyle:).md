

- Foundation
- FormatStyle
-  measurement(width:usage:numberFormatStyle:) 

Type Method

# measurement(width:usage:numberFormatStyle:)

Returns a format style to format measurement units.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func measurement(
    width: Measurement.FormatStyle.UnitWidth,
    usage: MeasurementFormatUnitUsage = .general,
    numberFormatStyle: FloatingPointFormatStyle? = nil
) -> Self where Self == Measurement.FormatStyle, UnitType : Dimension
```

## Parameters 

`width`  

The width — such as full names or abbreviations — with which to present units.

`usage`  

The contextual usage of the measurement unit, such as whether a length measurement applies to a road distance or a person’s height.

`numberFormatStyle`  

The format style with which to format the numeric part of the measurement.

## Return Value

A format style that formats measurements according to the given parameters.

## Discussion

Use the dot-notation form of this type method when the call point allows the use of Measurement.FormatStyle. You typically do this when calling the formatted(_:) method of Measurement.

The following example creates an array of Measurement values that represent distances measured in kilometers. It then uses formatted(_:) and the format style provided by this method to format the distances. The style specifies the asProvided usage to keep the formatted measurements in kilometers. Without this, a non-Metric locale such as the US would convert the kilometers to a locale-appropriate unit, such as miles.

```
let rawDistances: [Double] = [100, 1000, 10000, 100000, 1000000]
let distances = rawDistances.map { Measurement(value: $0, unit: UnitLength.kilometers) }
let formattedDistances = distances.map { $0.formatted(
    .measurement(width: .narrow,
                 usage: .asProvided,
                 numberFormatStyle: .number)) } // ["100km", "1,000km", "10,000km", "100,000km", "1,000,000km"]
```

## See Also

### Applying measurement styles

static func measurement(width: Measurement&lt;UnitTemperature>.FormatStyle.UnitWidth, usage: MeasurementFormatUnitUsage&lt;UnitTemperature>, hidesScaleName: Bool, numberFormatStyle: FloatingPointFormatStyle&lt;Double>?) -> Self

Returns a format style to format temperature units.

