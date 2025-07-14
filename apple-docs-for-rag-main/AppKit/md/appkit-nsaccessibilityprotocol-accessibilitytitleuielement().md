

- AppKit
- NSAccessibilityProtocol
-  accessibilityTitleUIElement() 

Instance Method

# accessibilityTitleUIElement()

Returns the static text element that represents the accessibility element’s title.

macOS 10.10+

``` source
func accessibilityTitleUIElement() -> Any?
```

**Required**

## See Also

### Configuring Linkage Elements

func accessibilityLinkedUIElements() -> [Any]?

Returns the elements that have links with the accessibility element.

**Required**

func setAccessibilityLinkedUIElements([Any]?)

Sets the elements that have links with the accessibility element.

**Required**

func accessibilityServesAsTitleForUIElements() -> [Any]?

Returns the list of elements that the accessibility element is a title for.

**Required**

func setAccessibilityServesAsTitleForUIElements([Any]?)

Sets the list of elements that the accessibility element is a title for.

**Required**

func setAccessibilityTitleUIElement(Any?)

Sets the static text element that represents the accessibility element’s title.

**Required**

