

- AppKit
- NSAccessibilityProtocol
-  accessibilityChildrenInNavigationOrder() 

Instance Method

# accessibilityChildrenInNavigationOrder()

Returns the array of child accessibility elements in order for linear navigation.

macOS 10.13+

``` source
func accessibilityChildrenInNavigationOrder() -> [any NSAccessibilityElementProtocol]?
```

**Required**

## See Also

### Determining Relationships

func accessibilityChildren() -> [Any]?

Returns the child accessibility elements in the accessibility hierarchy.

**Required**

func setAccessibilityChildren([Any]?)

Sets the child accessibility elements in the accessibility hierarchy.

**Required**

func setAccessibilityChildrenInNavigationOrder([any NSAccessibilityElementProtocol]?)

Sets the array of child accessibility elements in order for linear navigation.

**Required**

func accessibilityParent() -> Any?

Returns the accessibility element’s parent in the accessibility hierarchy.

**Required**

func setAccessibilityParent(Any?)

Sets the accessibility element’s parent in the accessibility hierarchy.

**Required**

func accessibilitySelectedChildren() -> [Any]?

Returns the accessibility element’s currently selected children.

**Required**

func setAccessibilitySelectedChildren([Any]?)

Sets the accessibility element’s currently selected children.

**Required**

func accessibilityTopLevelUIElement() -> Any?

Returns the top-level element that contains the accessibility element.

**Required**

func setAccessibilityTopLevelUIElement(Any?)

Sets the top-level element that contains the accessibility element.

**Required**

func accessibilityVisibleChildren() -> [Any]?

Returns the accessibility element’s visible child accessibility elements.

**Required**

func setAccessibilityVisibleChildren([Any]?)

Sets the accessibility element’s visible child accessibility elements.

**Required**

