

- AppKit
- NSTypesetter
-  paragraphSpacing(beforeGlyphAt:withProposedLineFragmentRect:) 

Instance Method

# paragraphSpacing(beforeGlyphAt:withProposedLineFragmentRect:)

Returns the number of points of space—added before a paragraph—that is in effect before the specified glyph.

macOS

``` source
func paragraphSpacing(
    beforeGlyphAt glyphIndex: Int,
    withProposedLineFragmentRect rect: NSRect
) -> CGFloat
```

## Parameters 

`glyphIndex`  

The index of the glyph in question.

`rect`  

The line fragment rectangle of the first line in the paragraph.

## Return Value

The number of points of space—added before a paragraph—that is in effect before the glyph specified by `glyphIndex`.

## Discussion

The typesetter adds the number of points specified in the return value to the top of the line fragment rectangle specified by `rect` (but not to the used line fragment rectangle for that line). Paragraph spacing added before a paragraph correlates to the value returned by the paragraphSpacingBefore method of NSParagraphStyle, which you can set using the paragraphSpacingBefore method of NSMutableParagraphStyle.

## See Also

### Getting spacing information

func lineSpacing(afterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the line spacing in effect following the specified glyph.

func paragraphSpacing(afterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the paragraph spacing that is in effect after the specified glyph.

