

- AppKit
- NSLayoutManager
-  boundsRect(for:at:effectiveRange:) 

Instance Method

# boundsRect(for:at:effectiveRange:)

Returns the bounding rectangle for the specified text block and glyph.

macOS 10.7+

``` source
func boundsRect(
    for block: NSTextBlock,
    at glyphIndex: Int,
    effectiveRange effectiveGlyphRange: NSRangePointer?
) -> NSRect
```

## Parameters 

`block`  

The text block whose bounding rectangle is returned.

`glyphIndex`  

Index of the glyph.

`effectiveGlyphRange`  

If not `NULL`, on output, the range for all glyphs in the text block.

## Return Value

The bounding rectangle of the text block, or `NSZeroRect` if no rectangle has been set for the specified block since the last invalidation.

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

func boundsRect(for: NSTextBlock, glyphRange: NSRange) -> NSRect

Returns the bounding rectangle that encloses the specified text block and glyph range.

func layoutRect(for: NSTextBlock, at: Int, effectiveRange: NSRangePointer?) -> NSRect

Returns the rectangle for the layout of the specified text block and glyph.

