

- Foundation
- NSMutableAttributedString
-  fixParagraphStyleAttribute(in:) 

Instance Method

# fixParagraphStyleAttribute(in:)

Fixes the paragraph style attributes in the specified range and assigns a paragraph style to all characters in the paragraph.

macOS 10.0+

``` source
func fixParagraphStyleAttribute(in range: NSRange)
```

## Parameters 

`range`  

The range of characters.

## Discussion

This method assigns the first paragraph style attribute value in each paragraph to all characters of the paragraph. This method extends the range as needed to cover the last paragraph partially contained. A paragraph is delimited by any of these characters, the longest possible sequence being preferred to any shorter:

- U+000D (`\r` or CR)

- U+000A (`\n` or LF)

- U+2029 (Unicode paragraph separator) `\r\n`, in that order (also known as CRLF)

Raises an rangeException if any part of `range` lies beyond the end of the receiver’s characters.

## See Also

### Fixing Attributes After Changes

func fixAttributes(in: NSRange)

Cleans up font, paragraph style, and attachment attributes within the given range.

func fixAttachmentAttribute(in: NSRange)

Cleans up attachment attributes in the specified range and removes all attachment attributes assigned to characters except the designated attachment character.

func fixFontAttribute(in: NSRange)

Fixes the font attribute in the specified range and assigns default fonts where appropriate.

