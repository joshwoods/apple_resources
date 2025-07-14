

- AppKit
- NSFont
-  getAdvancements(\_:forCGGlyphs:count:) 

Instance Method

# getAdvancements(\_:forCGGlyphs:count:)

Returns an array of the advancements for the specified glyphs rendered by the receiver.

macOS 10.13+

``` source
func getAdvancements(
    _ advancements: NSSizeArray,
    forCGGlyphs glyphs: UnsafePointer,
    count glyphCount: Int
)
```

## Discussion

Returns in `advancements` an array of the advancements for the glyphs specified by `glyphs` and rendered by the receiver. The `glyphCount` value must specify the count of glyphs passed in `glyphs`.

## See Also

### Getting Glyph Advancements

var maximumAdvancement: NSSize

The maximum advance of any of the font’s glyphs.

func advancement(forCGGlyph: CGGlyph) -> NSSize

Returns the nominal spacing for the given glyph—the distance the current point moves after showing the glyph—accounting for the receiver’s size.

