

- AppKit
- NSTypesetter
-  hyphenCharacter(forGlyphAt:) 

Instance Method

# hyphenCharacter(forGlyphAt:)

Returns the hyphen character to be inserted after the specified glyph.

macOS

``` source
func hyphenCharacter(forGlyphAt glyphIndex: Int) -> UTF32Char
```

## Parameters 

`glyphIndex`  

The index of the glyph in question.

## Return Value

The hyphen character to be inserted after the glyph at `glyphIndex`.

## Discussion

The typesetter calls this method before hyphenating. A subclass can override this method to return a different hyphen glyph.

## See Also

### Laying out glyphs

func layoutGlyphs(in: NSLayoutManager, startingAtGlyphIndex: Int, maxNumberOfLineFragments: Int, nextGlyphIndex: UnsafeMutablePointer&lt;Int>)

Lays out glyphs in the specified layout manager starting at a specified glyph.

Deprecated

func boundingBox(forControlGlyphAt: Int, for: NSTextContainer, proposedLineFragment: NSRect, glyphPosition: NSPoint, characterIndex: Int) -> NSRect

Returns the bounding rectangle for the specified control glyph with the specified parameters.

func getLineFragmentRect(NSRectPointer, usedRect: NSRectPointer, forParagraphSeparatorGlyphRange: NSRange, atProposedOrigin: NSPoint)

Calculates the line fragment rectangle and line fragment used rectangle for blank lines.

func getLineFragmentRect(NSRectPointer!, usedRect: NSRectPointer!, remaining: NSRectPointer!, forStartingGlyphAt: Int, proposedRect: NSRect, lineSpacing: CGFloat, paragraphSpacingBefore: CGFloat, paragraphSpacingAfter: CGFloat)

Calculates line fragment rectangle, line fragment used rectangle, and remaining rectangle for a line fragment.

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

