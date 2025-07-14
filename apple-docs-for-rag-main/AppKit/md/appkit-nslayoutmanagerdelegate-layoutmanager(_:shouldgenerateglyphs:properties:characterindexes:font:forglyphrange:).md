

- AppKit
- NSLayoutManagerDelegate
-  layoutManager(\_:shouldGenerateGlyphs:properties:characterIndexes:font:forGlyphRange:) 

Instance Method

# layoutManager(\_:shouldGenerateGlyphs:properties:characterIndexes:font:forGlyphRange:)

Enables customization of the initial glyph generation process.

macOS 10.11+

``` source
optional func layoutManager(
    _ layoutManager: NSLayoutManager,
    shouldGenerateGlyphs glyphs: UnsafePointer,
    properties props: UnsafePointer,
    characterIndexes charIndexes: UnsafePointer,
    font aFont: NSFont,
    forGlyphRange glyphRange: NSRange
) -> Int
```

## Parameters 

`layoutManager`  

The layout manager doing the layout.

`glyphs`  

A pointer to the layout manager’s glyph cache.

`props`  

A pointer to a buffer containing glyph properties for the glyphs in the cache.

`charIndexes`  

A pointer to the starting index for the characters in the text storage for which glyphs are generated.

`aFont`  

A font to override the font attributes in the text storage for the specified character range.

`glyphRange`  

The range of glyphs in the glyph cache to set.

## Return Value

The actual glyph range stored in this method. By returning `0`, it can indicate for the layout manager to do the default processing.

## Discussion

This message is sent whenever the layout manager is about to store the initial glyph information via setGlyphs(_:properties:characterIndexes:font:forGlyphRange:). To customize the initial glyph generation process, this method can invoke setGlyphs(_:properties:characterIndexes:font:forGlyphRange:) with modified glyph information.

Note

Querying glyph information surrounding `glyphRange` could lead to recursion since the data might not be available yet.

## See Also

### Invalidating glyphs and layout

func layoutManagerDidInvalidateLayout(NSLayoutManager)

Informs the delegate when the specified layout manager invalidates layout information (not glyph information).

func layoutManager(NSLayoutManager, shouldUse: NSLayoutManager.ControlCharacterAction, forControlCharacterAt: Int) -> NSLayoutManager.ControlCharacterAction

Returns the control character action for the control character at the specified character index.

struct ControlCharacterAction

Constants that describe actions for control characters.

