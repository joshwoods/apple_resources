

- AppKit
- NSLayoutManager
-  range(ofNominallySpacedGlyphsContaining:) 

Instance Method

# range(ofNominallySpacedGlyphsContaining:)

Returns the range of displayable glyphs that surround the glyph at the specified index.

macOS 10.7+

``` source
func range(ofNominallySpacedGlyphsContaining glyphIndex: Int) -> NSRange
```

## Parameters 

`glyphIndex`  

Index of the glyph to test.

## Return Value

The range of nominally spaced glyphs.

## Discussion

This method returns the range for the glyphs around the given glyph that can be displayed using only their advancements from the font, without pairwise kerning or other adjustments to spacing. The range returned begins with the first glyph, counting back from `glyphIndex`, that has a location set, and it continues up to, but does not include, the next glyph that has a location set.

Performs glyph generation and layout if needed.

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

