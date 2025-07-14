

- AppKit
- NSLayoutManager
-  lineFragmentUsedRect(forGlyphAt:effectiveRange:) 

Instance Method

# lineFragmentUsedRect(forGlyphAt:effectiveRange:)

Returns the usage rectangle for the line fragment and (optionally) returns the entire range of glyphs in that fragment.

macOS 10.7+

``` source
func lineFragmentUsedRect(
    forGlyphAt glyphIndex: Int,
    effectiveRange effectiveGlyphRange: NSRangePointer?
) -> NSRect
```

## Parameters 

`glyphIndex`  

The glyph for which to return the line fragment used rectangle.

`effectiveGlyphRange`  

If not `NULL`, on output, the range for all glyphs in the line fragment.

## Return Value

The used rectangle for the line fragment in which the given glyph is laid out.

## Discussion

This method causes glyph generation and layout for the line fragment containing the specified glyph, or if noncontiguous layout is not enabled, up to and including that line fragment.

Line fragment used rectangles are always in container coordinates.

Overriding this method is not recommended. If the line fragment used rectangle needs to be modified, that should be done at the typesetter level or by calling setLineFragmentRect(_:forGlyphRange:usedRect:).

## See Also

### Getting layout information

func attachmentSize(forGlyphAt: Int) -> NSSize

Returns the size of the attachment glyph at the specified index.

func drawsOutsideLineFragment(forGlyphAt: Int) -> Bool

Indicates whether the glyph draws outside its line fragment rectangle.

var extraLineFragmentRect: NSRect

The rectangle for the extra line fragment at the end of a document.

var extraLineFragmentTextContainer: NSTextContainer?

The text container for the extra line fragment rectangle.

var extraLineFragmentUsedRect: NSRect

The rectangle that encloses the insertion point in the extra line fragment rectangle.

func firstUnlaidCharacterIndex() -> Int

Returns the index for the first character in the layout manager that isn’t in the layout.

func firstUnlaidGlyphIndex() -> Int

Returns the index for the first glyph in the layout manager that isn’t in the layout.

func getFirstUnlaidCharacterIndex(UnsafeMutablePointer&lt;Int>?, glyphIndex: UnsafeMutablePointer&lt;Int>?)

Returns the indexes for the first character and glyph that have invalid layout information.

func lineFragmentRect(forGlyphAt: Int, effectiveRange: NSRangePointer?) -> NSRect

Returns the rectangle for the line fragment where the glyph lies and (optionally), by reference, the entire range of glyphs in that fragment.

func lineFragmentRect(forGlyphAt: Int, effectiveRange: NSRangePointer?, withoutAdditionalLayout: Bool) -> NSRect

Returns the line fragment rectangle that contains the glyph at the specified glyph index.

func lineFragmentUsedRect(forGlyphAt: Int, effectiveRange: NSRangePointer?, withoutAdditionalLayout: Bool) -> NSRect

Returns the usage rectangle for the line fragment and (optionally) returns the entire range of glyphs in that fragment.

func location(forGlyphAt: Int) -> NSPoint

Returns the location for the specified glyph within its line fragment.

func notShownAttribute(forGlyphAt: Int) -> Bool

Indicates whether the glyph at the specified index has a visible representation.

func truncatedGlyphRange(inLineFragmentForGlyphAt: Int) -> NSRange

Returns the range of truncated glyphs for a line fragment that contains the specified index.

