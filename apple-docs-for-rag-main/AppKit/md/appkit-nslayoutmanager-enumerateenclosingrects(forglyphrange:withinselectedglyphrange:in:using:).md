

- AppKit
- NSLayoutManager
-  enumerateEnclosingRects(forGlyphRange:withinSelectedGlyphRange:in:using:) 

Instance Method

# enumerateEnclosingRects(forGlyphRange:withinSelectedGlyphRange:in:using:)

Enumerates enclosing rectangles for the specified glyph range in a text container.

macOS 10.11+

``` source
func enumerateEnclosingRects(
    forGlyphRange glyphRange: NSRange,
    withinSelectedGlyphRange selectedRange: NSRange,
    in textContainer: NSTextContainer,
    using block: @escaping (NSRect, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`glyphRange`  

The glyph range for which to return enclosing rectangles.

`selectedRange`  

Selected glyphs within `glyphRange`, which can affect the size of the rectangles. If not interested in selection rectangles, pass `{NSNotFound, 0}` as the selected range.

`textContainer`  

The text container in which the glyphs are laid out.

`block`  

The block to apply to the glyph range. The block has two arguments:

rect  
The current enclosing rectangle.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the array. The stop argument is an out-only argument. You should only set this Boolean to true within the block.

## Discussion

These rectangles are always in container coordinates. They can be used to draw the text background or highlight for the given range of characters. The rectangles don’t necessarily enclose glyphs that draw outside their line fragment rectangles; use boundingRect(forGlyphRange:in:) to determine the area that contains all drawing performed for a range of glyphs.

If a selected range is given in the second argument, the rectangles returned are correct for drawing the selection. Selection rectangles are generally more complicated than enclosing rectangles, and supplying a selected range determines whether the method does this extra work. This method does the minimum amount of work required to answer the question.

Performs glyph generation and layout if needed.

## See Also

### Performing advanced layout queries

func boundingRect(forGlyphRange: NSRange, in: NSTextContainer) -> NSRect

Returns the bounding rectangle for the specified glyphs in a container.

func characterIndex(for: NSPoint, in: NSTextContainer, fractionOfDistanceBetweenInsertionPoints: UnsafeMutablePointer&lt;CGFloat>?) -> Int

Returns the index of the character that lies beneath the specified point using the specified container’s coordinate system.

func characterRange(forGlyphRange: NSRange, actualGlyphRange: NSRangePointer?) -> NSRange

Returns the range of characters that correspond to the glyphs in the specified glyph range.

func enumerateLineFragments(forGlyphRange: NSRange, using: (NSRect, NSRect, NSTextContainer, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates line fragments intersecting with the specified glyph range.

func fractionOfDistanceThroughGlyph(for: NSPoint, in: NSTextContainer) -> CGFloat

Returns the fraction of the distance between the glyph at the specified point and the next glyph.

func getLineFragmentInsertionPoints(forCharacterAt: Int, alternatePositions: Bool, inDisplayOrder: Bool, positions: UnsafeMutablePointer&lt;CGFloat>?, characterIndexes: UnsafeMutablePointer&lt;Int>?) -> Int

Returns insertion points in bulk for a specified line fragment.

func glyphIndex(for: NSPoint, in: NSTextContainer) -> Int

Returns the index of the glyph at the specified location in a text container.

func glyphIndex(for: NSPoint, in: NSTextContainer, fractionOfDistanceThroughGlyph: UnsafeMutablePointer&lt;CGFloat>?) -> Int

Returns the index of the glyph at the specified point using the container’s coordinate system.

func glyphRange(forBoundingRect: NSRect, in: NSTextContainer) -> NSRange

Returns the smallest contiguous range for glyphs lying wholly or partially within the specified rectangle of the text container.

func glyphRange(forBoundingRectWithoutAdditionalLayout: NSRect, in: NSTextContainer) -> NSRange

Returns the smallest contiguous range for glyphs lying wholly or partially within the specified rectangle of the text container.

func glyphRange(for: NSTextContainer) -> NSRange

Returns the range of glyphs lying within the specified text container.

func glyphRange(forCharacterRange: NSRange, actualCharacterRange: NSRangePointer?) -> NSRange

Returns the range of glyphs that the specified range of characters generates.

func range(ofNominallySpacedGlyphsContaining: Int) -> NSRange

Returns the range of displayable glyphs that surround the glyph at the specified index.

