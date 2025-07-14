

- AppKit
- NSTypesetter
-  hyphenationFactor(forGlyphAt:) 

Instance Method

# hyphenationFactor(forGlyphAt:)

Returns the hyphenation factor in effect at a specified location.

macOS

``` source
func hyphenationFactor(forGlyphAt glyphIndex: Int) -> Float
```

## Parameters 

`glyphIndex`  

The index of the glyph position to examine.

## Return Value

The hyphenation factor in effect at `glyphIndex`. The hyphenation factor is a value ranging from 0.0 to 1.0 that controls when hyphenation is attempted. By default, the value is 0.0, meaning hyphenation is off. A factor of 1.0 causes hyphenation to be attempted always.

## Discussion

The typesetter calls this method with a proposed hyphenation point for a line break to find the hyphenation factor in effect at that time. A subclass can override this method to customize the text layout process.

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

func hyphenCharacter(forGlyphAt: Int) -> UTF32Char

Returns the hyphen character to be inserted after the specified glyph.

func shouldBreakLine(byHyphenatingBeforeCharacterAt: Int) -> Bool

Returns whether the line being laid out should be broken by hyphenating at the specified character.

func shouldBreakLine(byWordBeforeCharacterAt: Int) -> Bool

Returns whether the line being laid out should be broken by a word break at the specified character.

func willSetLineFragmentRect(NSRectPointer, forGlyphRange: NSRange, usedRect: NSRectPointer, baselineOffset: UnsafeMutablePointer&lt;CGFloat>)

Called by the typesetter just prior to storing the actual line fragment rectangle location in the layout manager.

func setHardInvalidation(Bool, forGlyphRange: NSRange)

Sets whether to force the layout manager to invalidate the specified portion of the glyph cache when invalidating layout.

