

- Core Text
-  CTGlyphInfoCreateWithGlyphName(\_:\_:\_:) 

Function

# CTGlyphInfoCreateWithGlyphName(\_:\_:\_:)

Creates an immutable glyph info object with a glyph name.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTGlyphInfoCreateWithGlyphName(
    _ glyphName: CFString,
    _ font: CTFont,
    _ baseString: CFString
) -> CTGlyphInfo?
```

## Parameters 

`glyphName`  

The name of the glyph.

`font`  

The font to be associated with the returned CTGlyphInfo object.

`baseString`  

The part of the string the returned object is intended to override.

## Return Value

A valid reference to an immutable CTGlyphInfo object if glyph info creation was successful; otherwise, `NULL`.

## Discussion

This function creates an immutable glyph info object for a glyph name such as `copyright` using a specified font.

## See Also

### Creating GlyphInfo Objects

func CTGlyphInfoCreateWithGlyph(CGGlyph, CTFont, CFString) -> CTGlyphInfo?

Creates an immutable glyph info object with a glyph index.

func CTGlyphInfoCreateWithCharacterIdentifier(CGFontIndex, CTCharacterCollection, CFString) -> CTGlyphInfo?

Creates an immutable glyph info object with a character identifier.

