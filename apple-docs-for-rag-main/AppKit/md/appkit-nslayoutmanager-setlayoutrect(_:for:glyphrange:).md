

- AppKit
- NSLayoutManager
-  setLayoutRect(\_:for:glyphRange:) 

Instance Method

# setLayoutRect(\_:for:glyphRange:)

Sets the layout rectangle that encloses the specified text block and glyph range.

macOS 10.7+

``` source
func setLayoutRect(
    _ rect: NSRect,
    for block: NSTextBlock,
    glyphRange: NSRange
)
```

## Parameters 

`rect`  

The layout rectangle to set.

`block`  

The text block whose layout rectangle is set.

`glyphRange`  

The range of glyphs in the text block.

## Discussion

This method causes glyph generation but not layout. Block layout rectangles and bounds rectangles are always in container coordinates.

## See Also

### Handling layout for text blocks

func layoutRect(for: NSTextBlock, glyphRange: NSRange) -> NSRect

Returns the rectangle for the layout of the specified text block and glyph range.

func setBoundsRect(NSRect, for: NSTextBlock, glyphRange: NSRange)

Sets the bounding rectangle that encloses the specified text block and glyph range.

func boundsRect(for: NSTextBlock, glyphRange: NSRange) -> NSRect

Returns the bounding rectangle that encloses the specified text block and glyph range.

func layoutRect(for: NSTextBlock, at: Int, effectiveRange: NSRangePointer?) -> NSRect

Returns the rectangle for the layout of the specified text block and glyph.

func boundsRect(for: NSTextBlock, at: Int, effectiveRange: NSRangePointer?) -> NSRect

Returns the bounding rectangle for the specified text block and glyph.

