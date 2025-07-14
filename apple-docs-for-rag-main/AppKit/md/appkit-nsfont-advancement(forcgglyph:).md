

- AppKit
- NSFont
-  advancement(forCGGlyph:) 

Instance Method

# advancement(forCGGlyph:)

Returns the nominal spacing for the given glyph—the distance the current point moves after showing the glyph—accounting for the receiver’s size.

macOS 10.13+

``` source
func advancement(forCGGlyph glyph: CGGlyph) -> NSSize
```

## Parameters 

`glyph`  

The glyph whose advancement is returned.

## Return Value

The advancement spacing in points.

## Discussion

The spacing is given according to the glyph’s movement direction, which is either strictly horizontal or strictly vertical.

## See Also

### Getting Glyph Advancements

var maximumAdvancement: NSSize

The maximum advance of any of the font’s glyphs.

func getAdvancements(NSSizeArray, forCGGlyphs: UnsafePointer&lt;CGGlyph>, count: Int)

Returns an array of the advancements for the specified glyphs rendered by the receiver.

