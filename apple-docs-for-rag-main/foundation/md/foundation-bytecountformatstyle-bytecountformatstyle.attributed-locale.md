

- Foundation
- ByteCountFormatStyle
- ByteCountFormatStyle.Attributed
-  locale 

Instance Property

# locale

The locale to use to format the numeric part of the byte count.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var locale: Locale
```

## See Also

### Accessing style properties

var allowedUnits: ByteCountFormatStyle.Units

The units the format style can use to express the byte count.

var spellsOutZero: Bool

A Boolean value that indicates whether the format style should spell out zero-byte values as text.

var includesActualByteCount: Bool

A Boolean value that indicates whether the format style should include the exact byte count, in addition to expressing it in terms of units.

