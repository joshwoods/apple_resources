

- AppKit
- NSTypesetter
-  lineSpacing(afterGlyphAt:withProposedLineFragmentRect:) 

Instance Method

# lineSpacing(afterGlyphAt:withProposedLineFragmentRect:)

Returns the line spacing in effect following the specified glyph.

macOS

``` source
func lineSpacing(
    afterGlyphAt glyphIndex: Int,
    withProposedLineFragmentRect rect: NSRect
) -> CGFloat
```

## Parameters 

`glyphIndex`  

The index of the glyph in question.

`rect`  

The proposed line fragment rectangle.

## Return Value

The line spacing in effect following the glyph at `glyphIndex`.

## Discussion

The NSATSTypesetter calls this method to determine the number of points of space to include below the descenders in the used rectangle for the proposed line fragment rectangle `rect`.

Line spacing, also called leading, is an attribute of NSParagraphStyle, which you can set on an NSMutableParagraphStyle object. A font typically includes a default minimum line spacing metric used if none is set in the paragraph style.

If the typesetter behavior specified in the layout manager is `NSTypesetterOriginalBehavior`, the text system uses the original, private typesetter `NSSimpleHorizontalTypesetter`, which adds the line spacing above the ascender. Similarly, NSATSTypesetter adds the line spacing above the ascender if the value is negative.

## See Also

### Getting spacing information

func paragraphSpacing(afterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the paragraph spacing that is in effect after the specified glyph.

func paragraphSpacing(beforeGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the number of points of space—added before a paragraph—that is in effect before the specified glyph.

