

- AppKit
- NSFont
-  fontDescriptor 

Instance Property

# fontDescriptor

The font descriptor object for the font.

macOS

``` source
var fontDescriptor: NSFontDescriptor { get }
```

## Discussion

The font descriptor contains a mutable dictionary of optional attributes for creating an `NSFont` object. For more information about font descriptors, see NSFontDescriptor.

## See Also

### Getting Font Metrics and Information

var pointSize: CGFloat

The point size of the font.

var coveredCharacterSet: CharacterSet

The character set containing all of the nominal characters that the font can render.

var isFixedPitch: Bool

A Boolean value indicating whether all glyphs in the font have the same advancement.

var mostCompatibleStringEncoding: UInt

The string encoding that works best with the font.

Advanced Font Metrics

Retrieve details about ascender and descender heights, glyph bounding rectangles, glyph advancements, and more.

