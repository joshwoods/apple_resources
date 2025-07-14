

- Foundation
- Measurement
-  Measurement.AttributedStyle 

Structure

# Measurement.AttributedStyle

A type that provides localized representations of measurements with an attributed string.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@dynamicMemberLookup
struct AttributedStyle
```

Available when `UnitType` inherits `Dimension`.

## Overview

Use either the formatted() or the formatted(_:) instance method of Measurement to create an attributed string representation of a measurement.

The formatted() method generates a string using the default measurement format style.

## Topics

### Comparing Measurement Attributed Styles

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

static func == &lt;LeftHandSideType, RightHandSideType>(Measurement&lt;LeftHandSideType>, Measurement&lt;RightHandSideType>) -> Bool

Compare two measurements of the same `Dimension`.

### Structures

struct ByteCount

A format style that converts byte counts into attributed strings.

### Subscripts

subscript&lt;T>(dynamicMember _: KeyPath&lt;Measurement&lt;UnitType>.FormatStyle, T>) -> T

subscript&lt;T>(dynamicMember _: WritableKeyPath&lt;Measurement&lt;UnitType>.FormatStyle, T>) -> T

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable
- Sendable

## See Also

### Formatting a Measurement

func formatted() -> String

Generates a locale-aware string representation of a measurement using the default measurement format style.

func formatted&lt;S>(S) -> S.FormatOutput

Generates a locale-aware string representation of a measurement using the provided measurement format style.

struct FormatStyle

A type that provides localized representations of measurements.

