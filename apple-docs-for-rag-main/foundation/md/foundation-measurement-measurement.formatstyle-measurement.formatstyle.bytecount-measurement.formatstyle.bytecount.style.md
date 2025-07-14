

- Foundation
- Measurement
- Measurement.FormatStyle
- Measurement.FormatStyle.ByteCount
-  Measurement.FormatStyle.ByteCount.Style 

Type Alias

# Measurement.FormatStyle.ByteCount.Style

The type used to represent the style of the formatted byte count.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
typealias Style = ByteCountFormatStyle.Style
```

## Discussion

This format style uses the ByteCountFormatStyle.Style type to represent the byte-count style.

## See Also

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

var locale: Locale

The locale to use to format the numeric part of the byte count.

