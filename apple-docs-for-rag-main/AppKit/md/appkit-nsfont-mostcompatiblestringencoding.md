

- AppKit
- NSFont
-  mostCompatibleStringEncoding 

Instance Property

# mostCompatibleStringEncoding

The string encoding that works best with the font.

macOS

``` source
var mostCompatibleStringEncoding: UInt { get }
```

## Discussion

The string encoding in this property is the encoding with the fewest unmatched characters and glyphs in the font. If this value is NSASCIIStringEncoding, the font could not determine the correct encoding; you should assume the font can render only ASCII characters. The font uses heuristically well-known font encodings to determine the value of this property, so for nonstandard encodings the property may not contain the optimal string encoding.

You can use the data(using:) or data(using:allowLossyConversion:) methods of NSString to convert strings to this encoding.

## See Also

### Getting Font Metrics and Information

var pointSize: CGFloat

The point size of the font.

var coveredCharacterSet: CharacterSet

The character set containing all of the nominal characters that the font can render.

var fontDescriptor: NSFontDescriptor

The font descriptor object for the font.

var isFixedPitch: Bool

A Boolean value indicating whether all glyphs in the font have the same advancement.

Advanced Font Metrics

Retrieve details about ascender and descender heights, glyph bounding rectangles, glyph advancements, and more.

