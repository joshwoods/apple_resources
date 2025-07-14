

- Foundation
- Measurement
- Measurement.AttributedStyle
- Measurement.AttributedStyle.ByteCount
-  init(style:allowedUnits:spellsOutZero:includesActualByteCount:locale:) 

Initializer

# init(style:allowedUnits:spellsOutZero:includesActualByteCount:locale:)

Initializes an attributed byte count format style.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    style: Measurement.AttributedStyle.ByteCount.Style,
    allowedUnits: Measurement.AttributedStyle.ByteCount.Units,
    spellsOutZero: Bool,
    includesActualByteCount: Bool,
    locale: Locale
)
```

## Parameters 

`style`  

The style of byte count to express, such as memory or file system storage.

`allowedUnits`  

The units the format style can use to express the byte count.

`spellsOutZero`  

A Boolean value that indicates whether the format style should spell out zero-byte values as text, like `Zero kB`.

`includesActualByteCount`  

A Boolean value that indicates whether the format style should include the exact byte count, in addition to expressing it in terms of units. For example, `1 kB (1,024 bytes)`.

`locale`  

The locale to use to format the numeric part of the byte count.

