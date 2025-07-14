

- Foundation
-  ByteCountFormatStyle 

Structure

# ByteCountFormatStyle

A format style that provides string representations of byte counts.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ByteCountFormatStyle
```

## Overview

The following example creates an `Int` representing 1,024 bytes, and then formats it as an expression of memory storage, with the default byte count format style.

```
let count: Int64 = 1024
let formatted = count.formatted(.byteCount(style: .memory)) // "1 kB"
```

You can also customize a byte count format style, and use this to format one or more Int64 instances. The following example creates a format style to only use kilobyte units, and to spell out the exact byte count of the measurement.

```
let style = ByteCountFormatStyle(style: .memory,                                 
                                 allowedUnits: [.kb],
                                 spellsOutZero: true,
                                 includesActualByteCount: false,
                                 locale: Locale(identifier: "en_US"))
let counts: [Int64] = [0, 1024, 2048, 4096, 8192, 16384, 32768, 65536]
let formatted = counts.map ( {style.format($0) } ) // ["Zero kB", "1 kB", "2 kB", "4 kB", "8 kB", "16 kB", "32 kB", "64 kB"]
```

## Topics

### Creating a byte count style

init(style: ByteCountFormatStyle.Style, allowedUnits: ByteCountFormatStyle.Units, spellsOutZero: Bool, includesActualByteCount: Bool, locale: Locale)

Initializes a byte count format style.

struct Units

The units to use when formatting a byte count, such as kilobytes or gigabytes.

### Customizing style behavior

var style: ByteCountFormatStyle.Style

The semantic style the format style uses to represent a byte count value.

enum Style

The semantic style to use when formatting a byte count value.

### Accessing style properties

var allowedUnits: ByteCountFormatStyle.Units

The units the format style can use to express the byte count.

struct Units

The units to use when formatting a byte count, such as kilobytes or gigabytes.

var spellsOutZero: Bool

A Boolean value that indicates whether the format style should spell out zero-byte values as text.

var includesActualByteCount: Bool

A Boolean value that indicates whether the format style should include the exact byte count, in addition to expressing it in terms of units.

var locale: Locale

The locale to use to format the numeric part of the byte count.

### Creating attributed strings

var attributed: ByteCountFormatStyle.Attributed

An attributed format style based on the byte count format style.

struct Attributed

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

static func byteCount(style: Measurement&lt;UnitInformationStorage>.FormatStyle.ByteCount.Style, allowedUnits: Measurement&lt;UnitInformationStorage>.FormatStyle.ByteCount.Units, spellsOutZero: Bool, includesActualByteCount: Bool) -> Self

Returns a format style to format a data storage value represented with Foundation’s measurement type.

struct ByteCount

A format style that provides string representations of byte counts, expressed as measurements of information storage.

