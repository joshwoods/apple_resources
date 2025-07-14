

- AppKit
- NSAccessibilityProtocol
-  accessibilityServesAsTitleForUIElements() 

Instance Method

# accessibilityServesAsTitleForUIElements()

Returns the list of elements that the accessibility element is a title for.

macOS 10.10+

``` source
func accessibilityServesAsTitleForUIElements() -> [Any]?
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

func setAccessibilityServesAsTitleForUIElements([Any]?)

Sets the list of elements that the accessibility element is a title for.

**Required**

func accessibilityTitleUIElement() -> Any?

Returns the static text element that represents the accessibility element’s title.

**Required**

func setAccessibilityTitleUIElement(Any?)

Sets the static text element that represents the accessibility element’s title.

**Required**

