

- Foundation
- Measurement
-  Measurement.FormatStyle 

Structure

# Measurement.FormatStyle

A type that provides localized representations of measurements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct FormatStyle
```

Available when `UnitType` inherits `Dimension`.

## Overview

A measurement format style creates human-readable text from a Measurement. You can customize the formatting behavior of the format style using the width, `numberFormat`, usage, and locale properties. The system automatically caches unique configurations of Measurement.FormatStyle to enhance performance.

Use either the formatted() or the formatted(_:) instance method of Measurement to create a string representation of a measurement.

The formatted() method generates a string using the default measurement format style.

```
let temperature = Measurement(value: 38, unit: .celsius)
temperature.formatted()
// For locale: en_US: 100°F
// For locale: fr_FR: 38°C
```

The default format style in the previous example abbreviates the measurement unit. To customize any of the properties of the formatted measurement, you provide a measurement format style to the formatted(_:) method. For example, to create a string with the full name of the unit, the code might resemble the following:

```
temperature.formatted(.measurement(width: .wide))
// For locale: en_US: 100 degrees Fahrenheit
// For locale: fr_FR: 38 degrés Celsius
```

The previous example uses a static factory method to create a measurement format style within the call to the formatted(_:) method. You can also create a measurement format style and pass it to the method, such as in the following example:

```
let distance = Measurement(value: 36, unit: .miles)
let distanceStyle = Measurement.FormatStyle(width: .wide, usage: .road)
distanceStyle.format(distance)
// for locale: en_US: 36 miles
// for locale: fr_FR: 58 kilomètres

```

After you create an instance of a format style, you can use it to format measurements of the same unit type.

## Topics

### Creating a measurement format style

init(width: Measurement&lt;UnitType>.FormatStyle.UnitWidth, locale: Locale, usage: MeasurementFormatUnitUsage&lt;UnitType>, numberFormatStyle: FloatingPointFormatStyle&lt;Double>?)

Creates an instance using the provided width, locale, usage type, and number format.

init(width: Measurement&lt;UnitType>.FormatStyle.UnitWidth, locale: Locale, usage: MeasurementFormatUnitUsage&lt;UnitType>, hidesScaleName: Bool, numberFormatStyle: FloatingPointFormatStyle&lt;Double>?)

Creates an instance using the provided width, locale, usage type, number format, and the option to hide the unit name.

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

var locale: Locale

The locale of the format style.

### Inspecting a measurement format style

var attributed: Measurement&lt;UnitType>.AttributedStyle

The attributed style for the measurement format style.

### Applying byte count styles

Use this format style when the measurement’s unit type is information storage.

struct ByteCount

A format style that provides string representations of byte counts, expressed as measurements of information storage.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable
- Sendable

