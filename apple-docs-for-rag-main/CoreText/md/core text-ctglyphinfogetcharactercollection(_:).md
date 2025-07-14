

- Core Text
-  CTGlyphInfoGetCharacterCollection(\_:) 

Function

# CTGlyphInfoGetCharacterCollection(\_:)

Gets the character collection for a glyph info object.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CTGlyphInfoGetCharacterCollection(_ glyphInfo: CTGlyphInfo) -> CTCharacterCollection
```

## Parameters 

`glyphInfo`  

The glyph info from which to get the character collection. May not be `NULL`.

## Return Value

The character collection of the given glyph info object.

## Discussion

If the glyph info object was created with a glyph name or a glyph index, its character collection is kCTIdentityMappingCharacterCollection.

## See Also

### Getting GlyphInfo Data

func CTGlyphInfoGetGlyphName(CTGlyphInfo) -> CFString?

Retrieves the glyph name for a glyph info object, if that object exists.

func CTGlyphInfoGetCharacterIdentifier(CTGlyphInfo) -> CGFontIndex

Gets the character identifier for a glyph info object.

func CTGlyphInfoGetGlyph(CTGlyphInfo) -> CGGlyph

Retrieves the glyph for a glyph info, if that object exists.

