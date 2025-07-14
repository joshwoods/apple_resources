

- Core Graphics
-  CGFontPostScriptFormat 

Enumeration

# CGFontPostScriptFormat

Possible formats for a PostScript font subset.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
enum CGFontPostScriptFormat
```

## Topics

### Constants

case type1

A Type 1 font format.

case type3

A Type 3 PostScript format.

case type42

A constant representing a Type 42 font format.

### Initializers

init?(rawValue: Int32)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Working with PostScript Fonts

var postScriptName: CFString?

Obtains the PostScript name of a font.

func canCreatePostScriptSubset(CGFontPostScriptFormat) -> Bool

Determines whether Core Graphics can create a subset of the font in PostScript format.

func createPostScriptSubset(subsetName: CFString, format: CGFontPostScriptFormat, glyphs: UnsafePointer&lt;CGGlyph>?, count: Int, encoding: UnsafePointer&lt;CGGlyph>?) -> CFData?

Creates a subset of the font in the specified PostScript format.

func createPostScriptEncoding(encoding: UnsafePointer&lt;CGGlyph>?) -> CFData?

Creates a PostScript encoding of a font.

