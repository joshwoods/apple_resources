

- AppKit
- NSGlyphStorage
-  insertGlyphs(\_:length:forStartingGlyphAt:characterIndex:) 

Instance Method

# insertGlyphs(\_:length:forStartingGlyphAt:characterIndex:)

Inserts the given glyphs into the glyph cache and maps them to the specified characters.

macOS

``` source
func insertGlyphs(
    _ glyphs: UnsafePointer,
    length: Int,
    forStartingGlyphAt glyphIndex: Int,
    characterIndex charIndex: Int
)
```

**Required**

## Parameters 

`glyphs`  

The glyphs to insert.

`length`  

Number of glyphs to insert.

`glyphIndex`  

Location in the glyph cache to begin inserting glyphs.

`charIndex`  

Index of first character to be mapped.

## Discussion

This is a bulk insert method for the glyph cache.

## See Also

### Modifying the glyph cache

func setIntAttribute(Int, value: Int, forGlyphAt: Int)

Sets a custom attribute value for a given glyph.

**Required**

