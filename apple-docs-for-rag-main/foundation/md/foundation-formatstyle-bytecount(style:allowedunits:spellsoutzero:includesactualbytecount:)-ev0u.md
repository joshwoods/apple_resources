

- Foundation
- FormatStyle
-  byteCount(style:allowedUnits:spellsOutZero:includesActualByteCount:) 

Type Method

# byteCount(style:allowedUnits:spellsOutZero:includesActualByteCount:)

Returns a format style to format a data storage value represented with Foundation’s measurement type.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func byteCount(
    style: Measurement.FormatStyle.ByteCount.Style,
    allowedUnits: Measurement.FormatStyle.ByteCount.Units = .all,
    spellsOutZero: Bool = true,
    includesActualByteCount: Bool = false
) -> Self
```

Available when `Self` is `Measurement.FormatStyle.ByteCount`.

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

Use this type method when the call point allows the use of Measurement.FormatStyle.ByteCount. You typically do this when calling the formatted() on a Measurement whose unit type is UnitInformationStorage, as seen in the following example.

```
let count = Measurement(value: 1024, unit: UnitInformationStorage.bytes)
let formatted = count.formatted(.byteCount(style: .memory)) // "1 kB"
```

## See Also

### Applying byte-count styles

static func byteCount(style: ByteCountFormatStyle.Style, allowedUnits: ByteCountFormatStyle.Units, spellsOutZero: Bool, includesActualByteCount: Bool) -> Self

Returns a format style to format a data storage value.

struct ByteCountFormatStyle

A format style that provides string representations of byte counts.

struct ByteCount

A format style that provides string representations of byte counts, expressed as measurements of information storage.

