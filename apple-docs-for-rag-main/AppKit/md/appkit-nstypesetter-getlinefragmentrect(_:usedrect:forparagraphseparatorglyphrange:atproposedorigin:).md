

- AppKit
- NSTypesetter
-  getLineFragmentRect(\_:usedRect:forParagraphSeparatorGlyphRange:atProposedOrigin:) 

Instance Method

# getLineFragmentRect(\_:usedRect:forParagraphSeparatorGlyphRange:atProposedOrigin:)

Calculates the line fragment rectangle and line fragment used rectangle for blank lines.

macOS

``` source
func getLineFragmentRect(
    _ lineFragmentRect: NSRectPointer,
    usedRect lineFragmentUsedRect: NSRectPointer,
    forParagraphSeparatorGlyphRange paragraphSeparatorGlyphRange: NSRange,
    atProposedOrigin lineOrigin: NSPoint
)
```

## Parameters 

`lineFragmentRect`  

On return, the calculated line fragment rectangle.

`lineFragmentUsedRect`  

On return, the used rectangle (the portion of the line fragment rectangle that actually contains marks).

`paragraphSeparatorGlyphRange`  

The range of glyphs under consideration. A `paragraphSeparatorGlyphRange` with length 0 indicates an extra line fragment (which occurs if the last character in the paragraph is a line separator).

`lineOrigin`  

The origin point of the line fragment rectangle.

## See Also

### Laying out glyphs

func layoutGlyphs(in: NSLayoutManager, startingAtGlyphIndex: Int, maxNumberOfLineFragments: Int, nextGlyphIndex: UnsafeMutablePointer&lt;Int>)

Lays out glyphs in the specified layout manager starting at a specified glyph.

Deprecated

func boundingBox(forControlGlyphAt: Int, for: NSTextContainer, proposedLineFragment: NSRect, glyphPosition: NSPoint, characterIndex: Int) -> NSRect

Returns the bounding rectangle for the specified control glyph with the specified parameters.

func getLineFragmentRect(NSRectPointer!, usedRect: NSRectPointer!, remaining: NSRectPointer!, forStartingGlyphAt: Int, proposedRect: NSRect, lineSpacing: CGFloat, paragraphSpacingBefore: CGFloat, paragraphSpacingAfter: CGFloat)

Calculates line fragment rectangle, line fragment used rectangle, and remaining rectangle for a line fragment.

func hyphenCharacter(forGlyphAt: Int) -> UTF32Char

Returns the hyphen character to be inserted after the specified glyph.

func hyphenationFactor(forGlyphAt: Int) -> Float

Returns the hyphenation factor in effect at a specified location.

func shouldBreakLine(byHyphenatingBeforeCharacterAt: Int) -> Bool

Returns whether the line being laid out should be broken by hyphenating at the specified character.

func shouldBreakLine(byWordBeforeCharacterAt: Int) -> Bool

Returns whether the line being laid out should be broken by a word break at the specified character.

func willSetLineFragmentRect(NSRectPointer, forGlyphRange: NSRange, usedRect: NSRectPointer, baselineOffset: UnsafeMutablePointer&lt;CGFloat>)

Called by the typesetter just prior to storing the actual line fragment rectangle location in the layout manager.

func setHardInvalidation(Bool, forGlyphRange: NSRange)

Sets whether to force the layout manager to invalidate the specified portion of the glyph cache when invalidating layout.

