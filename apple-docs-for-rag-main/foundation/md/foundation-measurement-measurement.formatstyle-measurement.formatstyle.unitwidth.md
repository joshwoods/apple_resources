

- Foundation
- Measurement
- Measurement.FormatStyle
-  Measurement.FormatStyle.UnitWidth 

Structure

# Measurement.FormatStyle.UnitWidth

Specifies the width of the unit, determining the textual representation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct UnitWidth
```

## Topics

### Unit widths

static var wide: Measurement&lt;UnitType>.FormatStyle.UnitWidth

A unit width that shows the full unit name.

static var abbreviated: Measurement&lt;UnitType>.FormatStyle.UnitWidth

An abbreviated unit width.

static var narrow: Measurement&lt;UnitType>.FormatStyle.UnitWidth

The shortest unit width.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- Hashable
- Sendable

## See Also

### Modifying a measurement format style

var width: Measurement&lt;UnitType>.FormatStyle.UnitWidth

The width of the measurement unit.

var numberFormatStyle: FloatingPointFormatStyle&lt;Double>?

The formatting of the measurement value.

var usage: MeasurementFormatUnitUsage&lt;UnitType>?

The intended purpose of the formatted measurement.

var hidesScaleName: Bool

The visibility of the unit name of a temperature.

var locale: Locale

The locale of the format style.

