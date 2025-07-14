

- Core Text
-  CTFontGetLigatureCaretPositions(\_:\_:\_:\_:) 

Function

# CTFontGetLigatureCaretPositions(\_:\_:\_:\_:)

Returns caret positions within a glyph.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTFontGetLigatureCaretPositions(
    _ font: CTFont,
    _ glyph: CGGlyph,
    _ positions: UnsafeMutablePointer?,
    _ maxPositions: CFIndex
) -> CFIndex
```

## Parameters 

`font`  

A reference to the font to use.

`glyph`  

A reference to the glyph.

`positions`  

A buffer of at least `maxPositions` to receive the ligature caret positions for `glyph`.

`maxPositions`  

The maximum number of positions to return.

## Return Value

The maximum number of caret positions for the specified glyph

## Discussion

This function is used to obtain caret positions for a specific glyph. The return value is the maximum number of positions possible, and the function will populate the caller’s `positions` buffer with available positions if possible. This function might not be able to produce positions if the font does not have the appropriate data, in which case it will return 0.

## See Also

### Working with Glyphs

func CTFontGetGlyphsForCharacters(CTFont, UnsafePointer&lt;UniChar>, UnsafeMutablePointer&lt;CGGlyph>, CFIndex) -> Bool

Performs basic character-to-glyph mapping.

func CTFontDrawGlyphs(CTFont, UnsafePointer&lt;CGGlyph>, UnsafePointer&lt;CGPoint>, Int, CGContext)

Renders the given glyphs of a font at the specified positions in the supplied graphics context.

