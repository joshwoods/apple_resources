

- AppKit
- NSLayoutManager
-  layoutRect(for:glyphRange:) 

Instance Method

# layoutRect(for:glyphRange:)

Returns the rectangle for the layout of the specified text block and glyph range.

macOS 10.7+

``` source
func layoutRect(
    for block: NSTextBlock,
    glyphRange: NSRange
) -> NSRect
```

## Return Value

The layout rectangle, or `NSZeroRect` if no rectangle has been set for the specified block since the last invalidation.

## Discussion

This method causes glyph generation but not layout. Block layout rectangles and bounds rectangles are always in container coordinates.

## See Also

### Handling layout for text blocks

func setLayoutRect(NSRect, for: NSTextBlock, glyphRange: NSRange)

Sets the layout rectangle that encloses the specified text block and glyph range.

func setBoundsRect(NSRect, for: NSTextBlock, glyphRange: NSRange)

Sets the bounding rectangle that encloses the specified text block and glyph range.

func boundsRect(for: NSTextBlock, glyphRange: NSRange) -> NSRect

Returns the bounding rectangle that encloses the specified text block and glyph range.

func layoutRect(for: NSTextBlock, at: Int, effectiveRange: NSRangePointer?) -> NSRect

Returns the rectangle for the layout of the specified text block and glyph.

func boundsRect(for: NSTextBlock, at: Int, effectiveRange: NSRangePointer?) -> NSRect

Returns the bounding rectangle for the specified text block and glyph.

