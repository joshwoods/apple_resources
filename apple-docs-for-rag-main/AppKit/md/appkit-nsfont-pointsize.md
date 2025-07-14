

- AppKit
- NSFont
-  pointSize 

Instance Property

# pointSize

The point size of the font.

macOS

``` source
var pointSize: CGFloat { get }
```

## Discussion

If the font has a nonstandard matrix, the point size is the effective vertical point size.

## See Also

### Getting Font Metrics and Information

var coveredCharacterSet: CharacterSet

The character set containing all of the nominal characters that the font can render.

var fontDescriptor: NSFontDescriptor

The font descriptor object for the font.

var isFixedPitch: Bool

A Boolean value indicating whether all glyphs in the font have the same advancement.

var mostCompatibleStringEncoding: UInt

The string encoding that works best with the font.

Advanced Font Metrics

Retrieve details about ascender and descender heights, glyph bounding rectangles, glyph advancements, and more.

