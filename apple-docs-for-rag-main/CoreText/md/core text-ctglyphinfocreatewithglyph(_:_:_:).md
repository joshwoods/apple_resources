

- Core Text
-  CTGlyphInfoCreateWithGlyph(\_:\_:\_:) 

Function

# CTGlyphInfoCreateWithGlyph(\_:\_:\_:)

Creates an immutable glyph info object with a glyph index.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTGlyphInfoCreateWithGlyph(
    _ glyph: CGGlyph,
    _ font: CTFont,
    _ baseString: CFString
) -> CTGlyphInfo?
```

## Parameters 

`glyph`  

The index of the glyph.

`font`  

The font to be associated with the returned CTGlyphInfo object.

`baseString`  

The part of the string the returned object is intended to override.

## Return Value

A valid reference to an immutable CTGlyphInfo object, If glyph info creation was successful; otherwise, `NULL`.

## Discussion

This function creates an immutable glyph info object for a glyph index using a specified font.

## See Also

### Creating GlyphInfo Objects

func CTGlyphInfoCreateWithGlyphName(CFString, CTFont, CFString) -> CTGlyphInfo?

Creates an immutable glyph info object with a glyph name.

func CTGlyphInfoCreateWithCharacterIdentifier(CGFontIndex, CTCharacterCollection, CFString) -> CTGlyphInfo?

Creates an immutable glyph info object with a character identifier.

