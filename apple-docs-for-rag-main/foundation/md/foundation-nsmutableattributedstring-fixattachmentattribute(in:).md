

- Foundation
- NSMutableAttributedString
-  fixAttachmentAttribute(in:) 

Instance Method

# fixAttachmentAttribute(in:)

Cleans up attachment attributes in the specified range and removes all attachment attributes assigned to characters except the designated attachment character.

macOS 10.0+

``` source
func fixAttachmentAttribute(in range: NSRange)
```

## Parameters 

`range`  

The range of characters.

## Discussion

The method preserves the attachment attribute on the character special character. The method raises a rangeException if any part of `range` lies beyond the end of the string’s characters.

## See Also

### Fixing Attributes After Changes

func fixAttributes(in: NSRange)

Cleans up font, paragraph style, and attachment attributes within the given range.

func fixFontAttribute(in: NSRange)

Fixes the font attribute in the specified range and assigns default fonts where appropriate.

func fixParagraphStyleAttribute(in: NSRange)

Fixes the paragraph style attributes in the specified range and assigns a paragraph style to all characters in the paragraph.

