

- Foundation
- NSMutableAttributedString
-  addAttribute(\_:value:range:) 

Instance Method

# addAttribute(\_:value:range:)

Adds an attribute with the given name and value to the characters in the specified range.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func addAttribute(
    _ name: NSAttributedString.Key,
    value: Any,
    range: NSRange
)
```

## Parameters 

`name`  

A string specifying the attribute name. Attribute keys can be supplied by another framework or can be custom ones you define. For information about the system-supplied attribute keys, see the Constants section in NSAttributedString.

`value`  

The attribute value associated with `name`.

`range`  

The range of characters to which the specified attribute/value pair applies.

## Discussion

You may assign any `name`/`value` pair you wish to a range of characters. Raises an invalidArgumentException if `name` or `value` is `nil` and an rangeException if any part of `range` lies beyond the end of the receiver’s characters.

## See Also

### Changing Attributes

func setAttributes([NSAttributedString.Key : Any]?, range: NSRange)

Sets the attributes for the characters in the specified range to the specified attributes.

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

func unscriptRange(NSRange)

Removes the superscript attribute from the characters in the specified range.

