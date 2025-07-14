

- AppKit
- NSAccessibilityStaticText
-  accessibilityValue() 

Instance Method

# accessibilityValue()

Returns the text that the accessibility element displays.

macOS

``` source
func accessibilityValue() -> String?
```

**Required**

## Return Value

The text displayed by the element.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityValue property.

## See Also

### Supporting Accessibility

func accessibilityAttributedString(for: NSRange) -> NSAttributedString?

Returns the attributed substring for the specified range of characters.

func accessibilityVisibleCharacterRange() -> NSRange

Returns the range of visible characters in the document.

