

- Foundation
- NSMutableAttributedString
-  fixAttributes(in:) 

Instance Method

# fixAttributes(in:)

Cleans up font, paragraph style, and attachment attributes within the given range.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func fixAttributes(in range: NSRange)
```

## Parameters 

`range`  

The character range within which to fix attributes. Raises an rangeException if any part of `range` lies beyond the end of the receiver’s characters.

## Discussion

Removes attachment attributes assigned to characters other than character, assigns default fonts to characters with illegal fonts for their scripts and otherwise corrects font attribute assignments, and assigns the first paragraph style attribute value in each paragraph to all characters of the paragraph.

This method extends the range as needed to cover the last paragraph partially contained.

Raises an rangeException if any part of aRange lies beyond the end of the receiver’s characters.

`NSTextStorage` subclasses that return true from the fixesAttributesLazily method should avoid directly calling fixAttributes(in:) or else bracket such calls with beginEditing() and endEditing() messages.

## See Also

### Fixing Attributes After Changes

func fixAttachmentAttribute(in: NSRange)

Cleans up attachment attributes in the specified range and removes all attachment attributes assigned to characters except the designated attachment character.

func fixFontAttribute(in: NSRange)

Fixes the font attribute in the specified range and assigns default fonts where appropriate.

func fixParagraphStyleAttribute(in: NSRange)

Fixes the paragraph style attributes in the specified range and assigns a paragraph style to all characters in the paragraph.

