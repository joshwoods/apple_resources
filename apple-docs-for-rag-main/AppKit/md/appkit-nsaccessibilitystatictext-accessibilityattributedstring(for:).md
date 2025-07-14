

- AppKit
- NSAccessibilityStaticText
-  accessibilityAttributedString(for:) 

Instance Method

# accessibilityAttributedString(for:)

Returns the attributed substring for the specified range of characters.

macOS 10.0+

``` source
optional func accessibilityAttributedString(for range: NSRange) -> NSAttributedString?
```

## Parameters 

`range`  

The range of characters.

## Return Value

An attributed string representing the specified characters.

## See Also

### Supporting Accessibility

func accessibilityValue() -> String?

Returns the text that the accessibility element displays.

**Required**

func accessibilityVisibleCharacterRange() -> NSRange

Returns the range of visible characters in the document.

