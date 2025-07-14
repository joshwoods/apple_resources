

- AppKit
- NSFont
-  maximumAdvancement 

Instance Property

# maximumAdvancement

The maximum advance of any of the font’s glyphs.

macOS

``` source
var maximumAdvancement: NSSize { get }
```

## Discussion

The advancement is always either strictly horizontal or strictly vertical.

## See Also

### Related Documentation

func advancement(forGlyph: NSGlyph) -> NSSize

Returns the nominal spacing for the given glyph—the distance the current point moves after showing the glyph—accounting for the receiver’s size.

Deprecated

### Getting Glyph Advancements

func advancement(forCGGlyph: CGGlyph) -> NSSize

Returns the nominal spacing for the given glyph—the distance the current point moves after showing the glyph—accounting for the receiver’s size.

func getAdvancements(NSSizeArray, forCGGlyphs: UnsafePointer&lt;CGGlyph>, count: Int)

Returns an array of the advancements for the specified glyphs rendered by the receiver.

