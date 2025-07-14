

- AppKit
- NSTypesetter
-  willSetLineFragmentRect(\_:forGlyphRange:usedRect:baselineOffset:) 

Instance Method

# willSetLineFragmentRect(\_:forGlyphRange:usedRect:baselineOffset:)

Called by the typesetter just prior to storing the actual line fragment rectangle location in the layout manager.

macOS

``` source
func willSetLineFragmentRect(
    _ lineRect: NSRectPointer,
    forGlyphRange glyphRange: NSRange,
    usedRect: NSRectPointer,
    baselineOffset: UnsafeMutablePointer
)
```

## Parameters 

`lineRect`  

The rectangle in which the glyphs in `glyphRange` are laid out.

`glyphRange`  

The range of the glyphs to lay out.

`usedRect`  

The portion of `lineRect`, in the NSTextContainer object’s coordinate system, that actually contains glyphs or other marks that are drawn (including the text container’s line fragment padding). The `usedRect` must be equal to or contained within `lineRect`.

`baselineOffset`  

The vertical distance in pixels from the line fragment origin to the baseline on which the glyphs align.

## Discussion

Called by the typesetter just prior to calling setLineFragmentRect(_:forGlyphRange:usedRect:baselineOffset:) which stores the actual line fragment rectangle location in the layout manager.

A subclass can override this method to customize the text layout process. For example, it could change the shape of the line fragment rectangle. The subclass is responsible for ensuring that the modified rectangle remains valid (for example, that it lies within the text container).

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

func hyphenationFactor(forGlyphAt: Int) -> Float

Returns the hyphenation factor in effect at a specified location.

func shouldBreakLine(byHyphenatingBeforeCharacterAt: Int) -> Bool

Returns whether the line being laid out should be broken by hyphenating at the specified character.

func shouldBreakLine(byWordBeforeCharacterAt: Int) -> Bool

Returns whether the line being laid out should be broken by a word break at the specified character.

func setHardInvalidation(Bool, forGlyphRange: NSRange)

Sets whether to force the layout manager to invalidate the specified portion of the glyph cache when invalidating layout.

