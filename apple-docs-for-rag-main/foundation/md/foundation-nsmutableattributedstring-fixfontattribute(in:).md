

- Foundation
- NSMutableAttributedString
-  fixFontAttribute(in:) 

Instance Method

# fixFontAttribute(in:)

Fixes the font attribute in the specified range and assigns default fonts where appropriate.

macOS 10.0+

``` source
func fixFontAttribute(in range: NSRange)
```

## Parameters 

`range`  

The range of characters.

## Discussion

This method assigns default fonts to characters with illegal fonts for their scripts and corrects other font attribute assignments. For example, Kanji characters assigned a Latin font are reassigned an appropriate Kanji font. Raises an rangeException if any part of `range` lies beyond the end of the receiver’s characters.

## See Also

### Fixing Attributes After Changes

func fixAttributes(in: NSRange)

Cleans up font, paragraph style, and attachment attributes within the given range.

func fixAttachmentAttribute(in: NSRange)

Cleans up attachment attributes in the specified range and removes all attachment attributes assigned to characters except the designated attachment character.

func fixParagraphStyleAttribute(in: NSRange)

Fixes the paragraph style attributes in the specified range and assigns a paragraph style to all characters in the paragraph.

