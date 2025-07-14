

- AppKit
- NSFont
-  isFixedPitch 

Instance Property

# isFixedPitch

A Boolean value indicating whether all glyphs in the font have the same advancement.

macOS

``` source
var isFixedPitch: Bool { get }
```

## Discussion

The value of this property is true when all glyphs have the same advancement or false when they do not. Some Japanese fonts encoded with the scheme “EUC12-NJE-CFEncoding” return that they have the same advancement, but actually encode glyphs with one of two advancements, for historical compatibility. You may need to handle such fonts specially for some applications.

## See Also

### Related Documentation

func advancement(forGlyph: NSGlyph) -> NSSize

Returns the nominal spacing for the given glyph—the distance the current point moves after showing the glyph—accounting for the receiver’s size.

Deprecated

### Getting Font Metrics and Information

var pointSize: CGFloat

The point size of the font.

var coveredCharacterSet: CharacterSet

The character set containing all of the nominal characters that the font can render.

var fontDescriptor: NSFontDescriptor

The font descriptor object for the font.

var mostCompatibleStringEncoding: UInt

The string encoding that works best with the font.

Advanced Font Metrics

Retrieve details about ascender and descender heights, glyph bounding rectangles, glyph advancements, and more.

