

- AppKit
- NSLayoutManager
-  boundsRect(for:glyphRange:) 

Instance Method

# boundsRect(for:glyphRange:)

Returns the bounding rectangle that encloses the specified text block and glyph range.

macOS 10.7+

``` source
func boundsRect(
    for block: NSTextBlock,
    glyphRange: NSRange
) -> NSRect
```

## Parameters 

`block`  

The text block whose bounds rectangle is returned.

`glyphRange`  

The range of glyphs in the text block.

## Return Value

The bounding rectangle, or `NSZeroRect` if no rectangle has been set for the specified block since the last invalidation

## Discussion

This method causes glyph generation but not layout. Block layout rectangles and bounds rectangles are always in container coordinates.

## See Also

### Handling layout for text blocks

func setLayoutRect(NSRect, for: NSTextBlock, glyphRange: NSRange)

Sets the layout rectangle that encloses the specified text block and glyph range.

func layoutRect(for: NSTextBlock, glyphRange: NSRange) -> NSRect

Returns the rectangle for the layout of the specified text block and glyph range.

func setBoundsRect(NSRect, for: NSTextBlock, glyphRange: NSRange)

Sets the bounding rectangle that encloses the specified text block and glyph range.

func layoutRect(for: NSTextBlock, at: Int, effectiveRange: NSRangePointer?) -> NSRect

Returns the rectangle for the layout of the specified text block and glyph.

func boundsRect(for: NSTextBlock, at: Int, effectiveRange: NSRangePointer?) -> NSRect

Returns the bounding rectangle for the specified text block and glyph.

