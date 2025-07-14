

- UIKit
- NSLayoutManager
-  getLineFragmentInsertionPoints(forCharacterAt:alternatePositions:inDisplayOrder:positions:characterIndexes:) 

Instance Method

# getLineFragmentInsertionPoints(forCharacterAt:alternatePositions:inDisplayOrder:positions:characterIndexes:)

Returns insertion points in bulk for a specified line fragment.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func getLineFragmentInsertionPoints(
    forCharacterAt charIndex: Int,
    alternatePositions aFlag: Bool,
    inDisplayOrder dFlag: Bool,
    positions: UnsafeMutablePointer?,
    characterIndexes charIndexes: UnsafeMutablePointer?
) -> Int
```

## Parameters 

`charIndex`  

The character index of one character within the line fragment.

`aFlag`  

If true, returns alternate, rather than primary, insertion points.

`dFlag`  

If true, returns insertion points in display, rather than logical, order.

`positions`  

On output, the positions of the insertion points, in the order specified.

`charIndexes`  

On output, the indexes of the characters corresponding to the returned insertion points.

## Return Value

The number of insertion points returned.

## Discussion

The method allows clients to obtain all insertion points for a line fragment in one call. Each pointer passed in should either be `NULL` or else point to sufficient memory to hold as many elements as there are insertion points in the line fragment (which cannot be more than the number of characters + 1). The returned positions indicate a transverse offset relative to the line fragment rectangle’s origin. Internal caching is used to ensure that repeated calls to this method for the same line fragment (possibly with differing values for other arguments) are not significantly more expensive than a single call.

## See Also

### Related Documentation

func rectArray(forCharacterRange charRange: NSRange, withinSelectedCharacterRange selCharRange: NSRange, in container: NSTextContainer, rectCount: UnsafeMutablePointer&lt;Int>) -> NSRectArray?

Returns an array of rectangles and, by reference, the number of such rectangles, that define the region in the given container enclosing the given character range.

func rectArray(forGlyphRange glyphRange: NSRange, withinSelectedGlyphRange selGlyphRange: NSRange, in container: NSTextContainer, rectCount: UnsafeMutablePointer&lt;Int>) -> NSRectArray?

Returns an array of rectangles and, by reference, the number of such rectangles, that define the region in the given container enclosing the given glyph range.

### Performing advanced layout queries

func boundingRect(forGlyphRange: NSRange, in: NSTextContainer) -> CGRect

Returns the bounding rectangle for the specified glyphs in a container.

func characterIndex(for: CGPoint, in: NSTextContainer, fractionOfDistanceBetweenInsertionPoints: UnsafeMutablePointer&lt;CGFloat>?) -> Int

Returns the index of the character that lies beneath the specified point using the specified container’s coordinate system.

func characterRange(forGlyphRange: NSRange, actualGlyphRange: NSRangePointer?) -> NSRange

Returns the range of characters that correspond to the glyphs in the specified glyph range.

func enumerateEnclosingRects(forGlyphRange: NSRange, withinSelectedGlyphRange: NSRange, in: NSTextContainer, using: (CGRect, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates enclosing rectangles for the specified glyph range in a text container.

func enumerateLineFragments(forGlyphRange: NSRange, using: (CGRect, CGRect, NSTextContainer, NSRange, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates line fragments intersecting with the specified glyph range.

func fractionOfDistanceThroughGlyph(for: CGPoint, in: NSTextContainer) -> CGFloat

Returns the fraction of the distance between the glyph at the specified point and the next glyph.

func glyphIndex(for: CGPoint, in: NSTextContainer) -> Int

Returns the index of the glyph at the specified location in a text container.

func glyphIndex(for: CGPoint, in: NSTextContainer, fractionOfDistanceThroughGlyph: UnsafeMutablePointer&lt;CGFloat>?) -> Int

Returns the index of the glyph at the specified point using the container’s coordinate system.

func glyphRange(forBoundingRect: CGRect, in: NSTextContainer) -> NSRange

Returns the smallest contiguous range for glyphs lying wholly or partially within the specified rectangle of the text container.

func glyphRange(forBoundingRectWithoutAdditionalLayout: CGRect, in: NSTextContainer) -> NSRange

Returns the smallest contiguous range for glyphs lying wholly or partially within the specified rectangle of the text container.

func glyphRange(for: NSTextContainer) -> NSRange

Returns the range of glyphs lying within the specified text container.

func glyphRange(forCharacterRange: NSRange, actualCharacterRange: NSRangePointer?) -> NSRange

Returns the range of glyphs that the specified range of characters generates.

func range(ofNominallySpacedGlyphsContaining: Int) -> NSRange

Returns the range of displayable glyphs that surround the glyph at the specified index.

