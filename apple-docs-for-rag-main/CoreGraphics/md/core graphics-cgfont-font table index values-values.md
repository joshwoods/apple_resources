

- Core Graphics
- CGFont
-  Font Table Index Values 

API Collection

# Font Table Index Values

Possible values for an index into a font table.

## Overview

See CGFontIndex.

## Topics

### Constants

let kCGFontIndexMax: CGFontIndex

The maximum allowed value of a CGFontIndex.

let kCGFontIndexInvalid: CGFontIndex

An invalid font index (a value which never represents a valid glyph).

let kCGGlyphMax: CGFontIndex

The maximum allowed value of a CGGlyph.

## See Also

### Working with Font Tables

var tableTags: CFArray?

Returns an array of tags that correspond to the font tables for a font.

func table(for: UInt32) -> CFData?

Returns the font table that corresponds to the provided tag.

Obsolete Font Table Index Values

Deprecated values for an index into a font table.

