

- Foundation
- Measurement
- Measurement.AttributedStyle
- Measurement.AttributedStyle.ByteCount
-  Measurement.AttributedStyle.ByteCount.Units 

Type Alias

# Measurement.AttributedStyle.ByteCount.Units

The type the measurement format style uses to represent byte-counting units.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
typealias Units = ByteCountFormatStyle.Units
```

## Discussion

This format style uses the ByteCountFormatStyle.Units structure to represent the available units.

## See Also

### Accessing style properties

var allowedUnits: Measurement&lt;UnitInformationStorage>.AttributedStyle.ByteCount.Units

The units the format style can use to express the byte count.

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

