

- UIKit
- NSLayoutManager
-  notShownAttribute(forGlyphAt:) 

Instance Method

# notShownAttribute(forGlyphAt:)

Indicates whether the glyph at the specified index has a visible representation.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
func notShownAttribute(forGlyphAt glyphIndex: Int) -> Bool
```

## Parameters 

`glyphIndex`  

Index of the glyph.

## Return Value

true if the glyph at `glyphIndex` is not shown; otherwise false.

## Discussion

Some glyphs are not shown. For example, a tab, newline, or attachment glyph is not shown; it just affects the layout of following glyphs or locates the attachment graphic. Space characters, however, typically are shown as glyphs with a displacement, although they leave no visible marks.

This method causes glyph generation and layout for the line fragment containing the specified glyph, or if noncontiguous layout is not enabled, up to and including that line fragment.

Raises an `NSRangeException` if `glyphIndex` is out of bounds.

## See Also

### Related Documentation

func setNotShownAttribute(Bool, forGlyphAt: Int)

Sets the visibility of the glyph at the specified index.

### Getting layout information

func attachmentSize(forGlyphAt: Int) -> CGSize

Returns the size of the attachment glyph at the specified index.

func drawsOutsideLineFragment(forGlyphAt: Int) -> Bool

Indicates whether the glyph draws outside its line fragment rectangle.

var extraLineFragmentRect: CGRect

The rectangle for the extra line fragment at the end of a document.

var extraLineFragmentTextContainer: NSTextContainer?

The text container for the extra line fragment rectangle.

var extraLineFragmentUsedRect: CGRect

The rectangle that encloses the insertion point in the extra line fragment rectangle.

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

func truncatedGlyphRange(inLineFragmentForGlyphAt: Int) -> NSRange

Returns the range of truncated glyphs for a line fragment that contains the specified index.

