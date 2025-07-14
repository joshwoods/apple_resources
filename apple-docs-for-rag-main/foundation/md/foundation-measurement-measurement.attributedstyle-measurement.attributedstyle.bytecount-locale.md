

- Foundation
- Measurement
- Measurement.AttributedStyle
- Measurement.AttributedStyle.ByteCount
-  locale 

Instance Property

# locale

The locale to use to format the numeric part of the byte count.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var locale: Locale { get set }
```

## Discussion

To change the format style’s locale, use `Measurement/AttributedStyle/ByteCount/locale(_:)`.

## See Also

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

