

- AppKit
- NSLayoutManager
-  characterIndex(for:in:fractionOfDistanceBetweenInsertionPoints:) 

Instance Method

# characterIndex(for:in:fractionOfDistanceBetweenInsertionPoints:)

Returns the index of the character that lies beneath the specified point using the specified container’s coordinate system.

macOS 10.7+

``` source
func characterIndex(
    for point: NSPoint,
    in container: NSTextContainer,
    fractionOfDistanceBetweenInsertionPoints partialFraction: UnsafeMutablePointer?
) -> Int
```

## Parameters 

`point`  

The point to test.

`container`  

The text container within which the point is tested.

`partialFraction`  

A fraction of the distance from the insertion point, logically before the given character to the next one.

## Return Value

The index of the character falling under `point`.

## Discussion

Analogous to glyphIndex(for:in:fractionOfDistanceThroughGlyph:), but expressed in character index terms. The method returns the index of the character falling under `point`, expressed in coordinate system of `container`; if no character is under the point, the nearest character is returned, where nearest is defined according to the requirements of selection by mouse. However, this is not simply equivalent to taking the result of the corresponding glyph index method and converting it to a character index, because in some cases a single glyph represents more than one selectable character, for example an fi ligature glyph. In that case, there is an insertion point within the glyph, and this method returns one character or the other, depending on whether the specified point lies to the left or the right of that insertion point.

In general, this method returns only character indexes for which there is an insertion point. The `partialFraction` is a fraction of the distance from the insertion point, logically before the given character to the next one, which may be either to the right or to the left depending on directionality.

## See Also

### Performing advanced layout queries

func boundingRect(forGlyphRange: NSRange, in: NSTextContainer) -> NSRect

Returns the bounding rectangle for the specified glyphs in a container.

func characterRange(forGlyphRange: NSRange, actualGlyphRange: NSRangePointer?) -> NSRange

Returns the range of characters that correspond to the glyphs in the specified glyph range.

func enumerateEnclosingRects(forGlyphRange: NSRange, withinSelectedGlyphRange: NSRange, in: NSTextContainer, using: (NSRect, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates enclosing rectangles for the specified glyph range in a text container.

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

