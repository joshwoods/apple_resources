

- Core Text
-  CTFontDrawGlyphs(\_:\_:\_:\_:\_:) 

Function

# CTFontDrawGlyphs(\_:\_:\_:\_:\_:)

Renders the given glyphs of a font at the specified positions in the supplied graphics context.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontDrawGlyphs(
    _ font: CTFont,
    _ glyphs: UnsafePointer,
    _ positions: UnsafePointer,
    _ count: Int,
    _ context: CGContext
)
```

## Parameters 

`font`  

The font with glyphs to render. If the font has a size or matrix attribute, `context` is set with these values.

`glyphs`  

The glyphs to be rendered. The glyphs should be the result of proper Unicode text layout operations (such as with `CTLine`). Functions such as CTFontGetGlyphsForCharacters(_:_:_:_:) do not perform any Unicode text layout.

`positions`  

The positions (origins) for each glyph in `glyphs`. The positions are in user space. The number of positions passed in must match the number of glyphs (in `glyphs`).

`count`  

The number of glyphs to be rendered from the `glyphs` array.

`context`  

The graphics context used to render the glyphs.

## Discussion

This function modifies graphics state including font, text size, and text matrix if these attributes are specified in `font`. These attributes are not restored.

## See Also

### Working with Glyphs

func CTFontGetGlyphsForCharacters(CTFont, UnsafePointer&lt;UniChar>, UnsafeMutablePointer&lt;CGGlyph>, CFIndex) -> Bool

Performs basic character-to-glyph mapping.

func CTFontGetLigatureCaretPositions(CTFont, CGGlyph, UnsafeMutablePointer&lt;CGFloat>?, CFIndex) -> CFIndex

Returns caret positions within a glyph.

