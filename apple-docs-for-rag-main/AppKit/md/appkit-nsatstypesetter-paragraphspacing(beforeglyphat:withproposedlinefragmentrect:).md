

- AppKit
- NSATSTypesetter
-  paragraphSpacing(beforeGlyphAt:withProposedLineFragmentRect:) 

Instance Method

# paragraphSpacing(beforeGlyphAt:withProposedLineFragmentRect:)

Returns the number of points of space added before a paragraph, which is in effect before the specified glyph.

macOS

``` source
func paragraphSpacing(
    beforeGlyphAt glyphIndex: Int,
    withProposedLineFragmentRect rect: NSRect
) -> CGFloat
```

## Discussion

The `rect` argument specifies the line fragment rectangle of the first line in the paragraph.

The typesetter adds the number of points specified in the return value to the top of the line fragment rectangle specified by `rect` (but not to the used line fragment rectangle for that line). Paragraph spacing added before a paragraph correlates to the value in the paragraphSpacingBefore property of NSParagraphStyle. You can set the value of this property in an NSMutableParagraphStyle object.

## See Also

### Getting Spacing Information

func lineSpacing(afterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the line spacing in effect following the specified glyph.

func paragraphSpacing(afterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the number of points of space added following a paragraph, in effect after the specified glyph.

