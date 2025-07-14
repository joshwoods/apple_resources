

- Foundation
- FormatStyle
-  byteCount(style:allowedUnits:spellsOutZero:includesActualByteCount:) 

Type Method

# byteCount(style:allowedUnits:spellsOutZero:includesActualByteCount:)

Returns a format style to format a data storage value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func byteCount(
    style: ByteCountFormatStyle.Style,
    allowedUnits: ByteCountFormatStyle.Units = .all,
    spellsOutZero: Bool = true,
    includesActualByteCount: Bool = false
) -> Self
```

Available when `Self` is `ByteCountFormatStyle`.

## Parameters 

`style`  

The style of byte count to express, such as memory or file system storage.

`allowedUnits`  

The units the format style can use to express the byte count.

`spellsOutZero`  

A Boolean value that indicates whether the format style should spell out zero-byte values as text, like `Zero kB`.

`includesActualByteCount`  

A Boolean value that indicates whether the format style should include the exact byte count, in addition to expressing it in terms of units. For example, `1 kB (1,024 bytes)`.

## Return Value

A format style for formatting a measurement of data storage, customized with the provided behaviors.

## Discussion

Use this type method when the call point allows the use of ByteCountFormatStyle. You typically do this when calling the formatted(_:) method of BinaryInteger values that represent byte counts, as seen here:

```
let count: Int64 = 1024
let formatted = count.formatted(.byteCount(style: .memory)) // "1 kB"
```

## See Also

### Applying byte-count styles

struct ByteCountFormatStyle

A format style that provides string representations of byte counts.

static func byteCount(style: Measurement&lt;UnitInformationStorage>.FormatStyle.ByteCount.Style, allowedUnits: Measurement&lt;UnitInformationStorage>.FormatStyle.ByteCount.Units, spellsOutZero: Bool, includesActualByteCount: Bool) -> Self

Returns a format style to format a data storage value represented with Foundation’s measurement type.

struct ByteCount

A format style that provides string representations of byte counts, expressed as measurements of information storage.

