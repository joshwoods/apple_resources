

- Core Text
-  CTGlyphInfoGetCharacterIdentifier(\_:) 

Function

# CTGlyphInfoGetCharacterIdentifier(\_:)

Gets the character identifier for a glyph info object.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTGlyphInfoGetCharacterIdentifier(_ glyphInfo: CTGlyphInfo) -> CGFontIndex
```

## Parameters 

`glyphInfo`  

The glyph info from which to get the character identifier. May not be `NULL`.

## Return Value

The character identifier of the given glyph info object.

## See Also

### Getting GlyphInfo Data

func CTGlyphInfoGetGlyphName(CTGlyphInfo) -> CFString?

Retrieves the glyph name for a glyph info object, if that object exists.

func CTGlyphInfoGetCharacterCollection(CTGlyphInfo) -> CTCharacterCollection

Gets the character collection for a glyph info object.

func CTGlyphInfoGetGlyph(CTGlyphInfo) -> CGGlyph

Retrieves the glyph for a glyph info, if that object exists.

