

- AppKit
- NSGlyphGenerator
-  generateGlyphs(for:desiredNumberOfCharacters:glyphIndex:characterIndex:) 

Instance Method

# generateGlyphs(for:desiredNumberOfCharacters:glyphIndex:characterIndex:)

Generates glyphs for the specified glyph storage object (`NSLayoutManager` by default).

macOS

``` source
func generateGlyphs(
    for glyphStorage: any NSGlyphStorage,
    desiredNumberOfCharacters nChars: Int,
    glyphIndex: UnsafeMutablePointer?,
    characterIndex charIndex: UnsafeMutablePointer?
)
```

## Discussion

Generates glyphs for the glyph storage object specified by `glyphStorage`, beginning with the character at `charIndex` and continuing for `nChars` characters. The `glyphIndex` specifies the index of the first glyph generated.

