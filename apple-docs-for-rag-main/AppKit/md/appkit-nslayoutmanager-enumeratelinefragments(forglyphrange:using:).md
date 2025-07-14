

- AppKit
- NSLayoutManager
-  enumerateLineFragments(forGlyphRange:using:) 

Instance Method

# enumerateLineFragments(forGlyphRange:using:)

Enumerates line fragments intersecting with the specified glyph range.

macOS 10.11+

``` source
func enumerateLineFragments(
    forGlyphRange glyphRange: NSRange,
    using block: @escaping (NSRect, NSRect, NSTextContainer, NSRange, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`glyphRange`  

The glyph range for which to return line fragment rectangles.

`block`  

The block to apply to the glyph range. The block has five arguments:

rect  
The current line fragment rectangle.

usedRect  
The portion of the line fragment rectangle that actually contains glyphs or other marks that are drawn (including the text container’s line fragment padding).

textContainer  
The text container in which the glyphs are laid out.

glyphRange  
The range of glyphs laid out in the current line fragment.

stop  
A reference to a Boolean value. The block can set the value to true to stop further processing of the array. The stop argument is an out-only argument. You should only set this Boolean to true within the block.

## Discussion

This method causes glyph generation and layout for the line fragment containing the glyphs in the specified range, or if noncontiguous layout is not enabled, for all of the text up to and including that line fragment.

Line fragment rectangles are always in container coordinates.

## See Also

### Performing advanced layout queries

func boundingRect(forGlyphRange: NSRange, in: NSTextContainer) -> NSRect

Returns the bounding rectangle for the specified glyphs in a container.

func characterIndex(for: NSPoint, in: NSTextContainer, fractionOfDistanceBetweenInsertionPoints: UnsafeMutablePointer&lt;CGFloat>?) -> Int

Returns the index of the character that lies beneath the specified point using the specified container’s coordinate system.

func characterRange(forGlyphRange: NSRange, actualGlyphRange: NSRangePointer?) -> NSRange

Returns the range of characters that correspond to the glyphs in the specified glyph range.

func enumerateEnclosingRects(forGlyphRange: NSRange, withinSelectedGlyphRange: NSRange, in: NSTextContainer, using: (NSRect, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates enclosing rectangles for the specified glyph range in a text container.

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

