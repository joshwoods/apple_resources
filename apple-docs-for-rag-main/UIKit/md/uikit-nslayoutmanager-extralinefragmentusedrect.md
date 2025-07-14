

- UIKit
- NSLayoutManager
-  extraLineFragmentUsedRect 

Instance Property

# extraLineFragmentUsedRect

The rectangle that encloses the insertion point in the extra line fragment rectangle.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
var extraLineFragmentUsedRect: CGRect { get }
```

## Discussion

The rectangle is defined in the coordinate system of its `NSTextContainer`. `NSZeroRect` if there is no extra line fragment rectangle.

The extra line fragment used rectangle is twice as wide (or tall) as the text container’s line fragment padding, with the insertion point itself in the middle.

## See Also

### Related Documentation

func setExtraLineFragmentRect(CGRect, usedRect: CGRect, textContainer: NSTextContainer)

Sets the bounds and container for the extra line fragment.

### Getting layout information

func attachmentSize(forGlyphAt: Int) -> CGSize

Returns the size of the attachment glyph at the specified index.

func drawsOutsideLineFragment(forGlyphAt: Int) -> Bool

Indicates whether the glyph draws outside its line fragment rectangle.

var extraLineFragmentRect: CGRect

The rectangle for the extra line fragment at the end of a document.

var extraLineFragmentTextContainer: NSTextContainer?

The text container for the extra line fragment rectangle.

func firstUnlaidCharacterIndex() -> Int

Returns the index for the first character in the layout manager that isn’t in the layout.

func firstUnlaidGlyphIndex() -> Int

Returns the index for the first glyph in the layout manager that isn’t in the layout.

func getFirstUnlaidCharacterIndex(UnsafeMutablePointer&lt;Int>?, glyphIndex: UnsafeMutablePointer&lt;Int>?)

Returns the indexes for the first character and glyph that have invalid layout information.

func lineFragmentRect(forGlyphAt: Int, effectiveRange: NSRangePointer?) -> CGRect

Returns the rectangle for the line fragment where the glyph lies and (optionally), by reference, the entire range of glyphs in that fragment.

func lineFragmentRect(forGlyphAt: Int, effectiveRange: NSRangePointer?, withoutAdditionalLayout: Bool) -> CGRect

Returns the line fragment rectangle that contains the glyph at the specified glyph index.

func lineFragmentUsedRect(forGlyphAt: Int, effectiveRange: NSRangePointer?) -> CGRect

Returns the usage rectangle for the line fragment and (optionally) returns the entire range of glyphs in that fragment.

func lineFragmentUsedRect(forGlyphAt: Int, effectiveRange: NSRangePointer?, withoutAdditionalLayout: Bool) -> CGRect

Returns the usage rectangle for the line fragment and (optionally) returns the entire range of glyphs in that fragment.

func location(forGlyphAt: Int) -> CGPoint

Returns the location for the specified glyph within its line fragment.

func notShownAttribute(forGlyphAt: Int) -> Bool

Indicates whether the glyph at the specified index has a visible representation.

func truncatedGlyphRange(inLineFragmentForGlyphAt: Int) -> NSRange

Returns the range of truncated glyphs for a line fragment that contains the specified index.

