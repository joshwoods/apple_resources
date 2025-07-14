

- AppKit
- NSLayoutManager
-  setBoundsRect(\_:for:glyphRange:) 

Instance Method

# setBoundsRect(\_:for:glyphRange:)

Sets the bounding rectangle that encloses the specified text block and glyph range.

macOS 10.7+

``` source
func setBoundsRect(
    _ rect: NSRect,
    for block: NSTextBlock,
    glyphRange: NSRange
)
```

## Parameters 

`rect`  

The bounding rectangle to set.

`block`  

The text block whose bounding rectangle is set.

`glyphRange`  

The range of glyphs in the text block.

## Discussion

This method causes glyph generation but not layout. Block layout rectangles and bounds rectangles are always in container coordinates.

## See Also

### Handling layout for text blocks

func setLayoutRect(NSRect, for: NSTextBlock, glyphRange: NSRange)

Sets the layout rectangle that encloses the specified text block and glyph range.

func layoutRect(for: NSTextBlock, glyphRange: NSRange) -> NSRect

Returns the rectangle for the layout of the specified text block and glyph range.

func boundsRect(for: NSTextBlock, glyphRange: NSRange) -> NSRect

Returns the bounding rectangle that encloses the specified text block and glyph range.

func layoutRect(for: NSTextBlock, at: Int, effectiveRange: NSRangePointer?) -> NSRect

Returns the rectangle for the layout of the specified text block and glyph.

func boundsRect(for: NSTextBlock, at: Int, effectiveRange: NSRangePointer?) -> NSRect

Returns the bounding rectangle for the specified text block and glyph.

