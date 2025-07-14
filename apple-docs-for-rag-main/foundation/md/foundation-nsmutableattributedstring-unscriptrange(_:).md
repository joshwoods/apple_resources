

- Foundation
- NSMutableAttributedString
-  unscriptRange(\_:) 

Instance Method

# unscriptRange(\_:)

Removes the superscript attribute from the characters in the specified range.

macOS 10.0+

``` source
func unscriptRange(_ range: NSRange)
```

## Parameters 

`range`  

The range of characters.

## Discussion

Raises an rangeException if any part of `range` lies beyond the end of the receiver’s characters.

## See Also

### Changing Attributes

func setAttributes([NSAttributedString.Key : Any]?, range: NSRange)

Sets the attributes for the characters in the specified range to the specified attributes.

func addAttribute(NSAttributedString.Key, value: Any, range: NSRange)

Adds an attribute with the given name and value to the characters in the specified range.

func addAttributes([NSAttributedString.Key : Any], range: NSRange)

Adds the given collection of attributes to the characters in the specified range.

func removeAttribute(NSAttributedString.Key, range: NSRange)

Removes the named attribute from the characters in the specified range.

func applyFontTraits(NSFontTraitMask, range: NSRange)

Applies the specified font-related attributes to characters in the string.

func setAlignment(NSTextAlignment, range: NSRange)

Sets the alignment characteristic of the paragraph style attribute for the specified range of text.

func setBaseWritingDirection(NSWritingDirection, range: NSRange)

Sets the base writing direction for the characters to the specified direction.

func subscriptRange(NSRange)

Decrements the value of the superscript attribute for characters in the specified range by one.

func superscriptRange(NSRange)

Increments the value of the superscript attribute for characters in the specified range by one.

