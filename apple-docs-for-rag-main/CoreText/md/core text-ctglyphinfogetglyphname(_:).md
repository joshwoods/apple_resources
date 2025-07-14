

- Core Text
-  CTGlyphInfoGetGlyphName(\_:) 

Function

# CTGlyphInfoGetGlyphName(\_:)

Retrieves the glyph name for a glyph info object, if that object exists.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTGlyphInfoGetGlyphName(_ glyphInfo: CTGlyphInfo) -> CFString?
```

## Parameters 

`glyphInfo`  

The glyph info object from which to get the glyph name. This parameter must not be `NULL`.

## Return Value

A glyph name, if the glyph info object was created with a name; otherwise, `NULL`.

## See Also

### Getting GlyphInfo Data

func CTGlyphInfoGetCharacterIdentifier(CTGlyphInfo) -> CGFontIndex

Gets the character identifier for a glyph info object.

func CTGlyphInfoGetCharacterCollection(CTGlyphInfo) -> CTCharacterCollection

Gets the character collection for a glyph info object.

func CTGlyphInfoGetGlyph(CTGlyphInfo) -> CGGlyph

Retrieves the glyph for a glyph info, if that object exists.

