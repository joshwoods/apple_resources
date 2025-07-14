

- Foundation
- Measurement
- Measurement.FormatStyle
-  Measurement.FormatStyle.ByteCount 

Structure

# Measurement.FormatStyle.ByteCount

A format style that provides string representations of byte counts, expressed as measurements of information storage.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct ByteCount
```

Available when `UnitType` is `UnitInformationStorage`.

## Overview

Use this style with a Measurement whose unit type is UnitInformationStorage to format byte counts according to locale conventions.

The following example creates a measurement of 1,024 bytes, and then formats it as an expression of memory storage, with the default byte count format style:

```
let count = Measurement(value: 1024, unit: UnitInformationStorage.bytes)
let formatted = count.formatted(.byteCount(style: .memory)) // "1 kB"
```

You can also customize a byte count format style, and use this to format one or more Measurement instances. The following example creates a format style to only use kilobyte units, and to spell out the exact byte count of the measurement.

```
let count = Measurement(value: 1024, unit: UnitInformationStorage.bytes)
let style = Measurement.FormatStyle.ByteCount(style: .memory,
                                              allowedUnits: .kb,
                                              spellsOutZero: true,
                                              includesActualByteCount: true,
                                              locale: Locale(identifier: "en_US"))
let customFormatted = style.format(count) // "1 kB (1,024 bytes)"
```

## Topics

### Creating a byte count style

init(style: Measurement&lt;UnitType>.FormatStyle.ByteCount.Style, allowedUnits: Measurement&lt;UnitType>.FormatStyle.ByteCount.Units, spellsOutZero: Bool, includesActualByteCount: Bool, locale: Locale)

Initializes a byte count format style.

### Accessing style properties

var allowedUnits: Measurement&lt;UnitInformationStorage>.FormatStyle.ByteCount.Units

The units the format style can use to express the byte count.

typealias Units

The type the measurement format style uses to represent byte-counting units.

var spellsOutZero: Bool

A Boolean value that indicates whether the format style should spell out zero-byte values as text.

var includesActualByteCount: Bool

A Boolean value that indicates whether the format style should include the exact byte count, in addition to expressing it in terms of units.

var style: Measurement&lt;UnitInformationStorage>.FormatStyle.ByteCount.Style

The style of byte count to express, such as memory or file system storage.

typealias Style

The type used to represent the style of the formatted byte count.

var locale: Locale

The locale to use to format the numeric part of the byte count.

### Creating attributed strings

var attributed: Measurement&lt;UnitInformationStorage>.AttributedStyle.ByteCount

An attributed format style based on the byte count format style.

struct ByteCount

A format style that converts byte counts into attributed strings.

## Relationships

### Conforms To

- Decodable
- Encodable
- Equatable
- FormatStyle
- Hashable
- Sendable

## See Also

### Applying byte-count styles

static func byteCount(style: ByteCountFormatStyle.Style, allowedUnits: ByteCountFormatStyle.Units, spellsOutZero: Bool, includesActualByteCount: Bool) -> Self

Returns a format style to format a data storage value.

struct ByteCountFormatStyle

A format style that provides string representations of byte counts.

static func byteCount(style: Measurement&lt;UnitInformationStorage>.FormatStyle.ByteCount.Style, allowedUnits: Measurement&lt;UnitInformationStorage>.FormatStyle.ByteCount.Units, spellsOutZero: Bool, includesActualByteCount: Bool) -> Self

Returns a format style to format a data storage value represented with Foundation’s measurement type.

