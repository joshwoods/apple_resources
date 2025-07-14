

- AppKit
- NSTypesetter
-  paragraphSpacing(afterGlyphAt:withProposedLineFragmentRect:) 

Instance Method

# paragraphSpacing(afterGlyphAt:withProposedLineFragmentRect:)

Returns the paragraph spacing that is in effect after the specified glyph.

macOS

``` source
func paragraphSpacing(
    afterGlyphAt glyphIndex: Int,
    withProposedLineFragmentRect rect: NSRect
) -> CGFloat
```

## Parameters 

`glyphIndex`  

The index of the glyph in question.

`rect`  

The line fragment rectangle of the last line in the paragraph.

## Return Value

The paragraph spacing—that is, the number of points of space added following a paragraph—that is in effect after the glyph specified by `glyphIndex`.

## Discussion

The typesetter adds the number of points specified in the return value to the bottom of the line fragment rectangle specified by `rect` (but not to the used line fragment rectangle for that line). Paragraph spacing added after a paragraph correlates to the value returned by the paragraphSpacing method of NSParagraphStyle, which you can set using the paragraphSpacing method of NSMutableParagraphStyle.

## See Also

### Getting spacing information

func lineSpacing(afterGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the line spacing in effect following the specified glyph.

func paragraphSpacing(beforeGlyphAt: Int, withProposedLineFragmentRect: NSRect) -> CGFloat

Returns the number of points of space—added before a paragraph—that is in effect before the specified glyph.

