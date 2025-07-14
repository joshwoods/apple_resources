

- AppKit
- NSLayoutManager
-  fractionOfDistanceThroughGlyph(for:in:) 

Instance Method

# fractionOfDistanceThroughGlyph(for:in:)

Returns the fraction of the distance between the glyph at the specified point and the next glyph.

macOS 10.7+

``` source
func fractionOfDistanceThroughGlyph(
    for point: NSPoint,
    in container: NSTextContainer
) -> CGFloat
```

## Discussion

This method is a primitive for glyphIndex(for:in:fractionOfDistanceThroughGlyph:). You should always call the main method, not the primitives.

Overriding should be done for the primitive methods. Existing subclasses that do not do this overriding will not have their implementations available to Java developers.

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

func enumerateLineFragments(forGlyphRange: NSRange, using: (NSRect, NSRect, NSTextContainer, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates line fragments intersecting with the specified glyph range.

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

