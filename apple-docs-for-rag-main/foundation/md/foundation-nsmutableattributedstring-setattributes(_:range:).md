

- Foundation
- NSMutableAttributedString
-  setAttributes(\_:range:) 

Instance Method

# setAttributes(\_:range:)

Sets the attributes for the characters in the specified range to the specified attributes.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setAttributes(
    _ attrs: [NSAttributedString.Key : Any]?,
    range: NSRange
)
```

## Parameters 

`attrs`  

A dictionary containing the attributes to set. Attribute keys can be supplied by another framework or can be custom ones you define. For information about the system-supplied attribute keys, see the Constants section in NSAttributedString.

`range`  

The range of characters whose attributes are set.

## Discussion

These new attributes replace any attributes previously associated with the characters in `range`. Raises an rangeException if any part of `range` lies beyond the end of the receiver’s characters.

To set attributes for a zero-length `NSMutableAttributedString` displayed in a text view, use the `NSTextView` method typingAttributes.

## See Also

### Changing Attributes

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

func unscriptRange(NSRange)

Removes the superscript attribute from the characters in the specified range.

