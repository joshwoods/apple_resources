

- Foundation
- Measurement
- Measurement.AttributedStyle
-  Measurement.AttributedStyle.ByteCount 

Structure

# Measurement.AttributedStyle.ByteCount

A format style that converts byte counts into attributed strings.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ByteCount
```

Available when `UnitType` is `UnitInformationStorage`.

## Overview

Use the attributed modifier on a Measurement.FormatStyle.ByteCount instance to create a format style of this type.

The attributed strings that this fomat style creates contain attributes from the AttributeScopes.FoundationAttributes.NumberFormatAttributes attribute scope. Use these attributes to determine which runs of the attributed string represent different parts of the formatted value.

## Topics

### Creating an attributed byte count format style

init(style: Measurement&lt;UnitType>.AttributedStyle.ByteCount.Style, allowedUnits: Measurement&lt;UnitType>.AttributedStyle.ByteCount.Units, spellsOutZero: Bool, includesActualByteCount: Bool, locale: Locale)

Initializes an attributed byte count format style.

### Accessing style properties

var allowedUnits: Measurement&lt;UnitInformationStorage>.AttributedStyle.ByteCount.Units

The units the format style can use to express the byte count.

typealias Units

The type the measurement format style uses to represent byte-counting units.

var spellsOutZero: Bool

A Boolean value that indicates whether the format style should spell out zero-byte values as text.

var includesActualByteCount: Bool

A Boolean value that indicates whether the format style should include the exact byte count, in addition to expressing it in terms of units.

var style: Measurement&lt;UnitInformationStorage>.AttributedStyle.ByteCount.Style

The style of byte count to express, such as memory or file system storage.

typealias Style

The type used to represent the style of the formatted byte count.

var locale: Locale

The locale to use to format the numeric part of the byte count.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable
- Sendable

## See Also

### Creating attributed strings

var attributed: Measurement&lt;UnitInformationStorage>.AttributedStyle.ByteCount

An attributed format style based on the byte count format style.

