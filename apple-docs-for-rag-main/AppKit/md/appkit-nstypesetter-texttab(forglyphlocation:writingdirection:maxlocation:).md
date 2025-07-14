

- AppKit
- NSTypesetter
-  textTab(forGlyphLocation:writingDirection:maxLocation:) 

Instance Method

# textTab(forGlyphLocation:writingDirection:maxLocation:)

Returns the text tab next closest to a given glyph location within the given parameters.

macOS

``` source
func textTab(
    forGlyphLocation glyphLocation: CGFloat,
    writingDirection direction: NSWritingDirection,
    maxLocation: CGFloat
) -> NSTextTab?
```

## Parameters 

`glyphLocation`  

The location at which to start searching.

`direction`  

The direction in which to search.

`maxLocation`  

The maximum location for the search.

## Return Value

The text tab next closest to `glyphLocation`, indexing in `direction` but not beyond `maxLocation`.

## Discussion

The typesetter calls this method whenever it finds a tab character. To determine the width to advance the next glyph, the typesetter examines the NSParagraphStyle object’s tab array and the default tab interval.

