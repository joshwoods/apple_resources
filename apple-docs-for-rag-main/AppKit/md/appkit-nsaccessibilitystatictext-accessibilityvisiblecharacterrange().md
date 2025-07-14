

- AppKit
- NSAccessibilityStaticText
-  accessibilityVisibleCharacterRange() 

Instance Method

# accessibilityVisibleCharacterRange()

Returns the range of visible characters in the document.

macOS

``` source
optional func accessibilityVisibleCharacterRange() -> NSRange
```

## Return Value

The range of the visible characters in the document. This method should return the range for entire lines. Characters that are horizontally clipped are included in this range.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityVisibleCharacterRange property.

## See Also

### Supporting Accessibility

func accessibilityAttributedString(for: NSRange) -> NSAttributedString?

Returns the attributed substring for the specified range of characters.

func accessibilityValue() -> String?

Returns the text that the accessibility element displays.

**Required**

