

- Core Text
-  CTGlyphInfoGetGlyph(\_:) 

Function

# CTGlyphInfoGetGlyph(\_:)

Retrieves the glyph for a glyph info, if that object exists.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func CTGlyphInfoGetGlyph(_ glyphInfo: CTGlyphInfo) -> CGGlyph
```

## Parameters 

`glyphInfo`  

The glyph info object from which to get the glyph.

## Return Value

A CGGlyph value, if the glyph info object was created with a font; otherwise, `0`.

## See Also

### Getting GlyphInfo Data

func CTGlyphInfoGetGlyphName(CTGlyphInfo) -> CFString?

Retrieves the glyph name for a glyph info object, if that object exists.

func CTGlyphInfoGetCharacterIdentifier(CTGlyphInfo) -> CGFontIndex

Gets the character identifier for a glyph info object.

func CTGlyphInfoGetCharacterCollection(CTGlyphInfo) -> CTCharacterCollection

Gets the character collection for a glyph info object.

