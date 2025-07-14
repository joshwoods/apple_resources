

- AppKit
- NSAccessibilityProtocol
-  setAccessibilityVisibleChildren(\_:) 

Instance Method

# setAccessibilityVisibleChildren(\_:)

Sets the accessibility element’s visible child accessibility elements.

macOS 10.10+

``` source
func setAccessibilityVisibleChildren(_ accessibilityVisibleChildren: [Any]?)
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

func accessibilityChildrenInNavigationOrder() -> [any NSAccessibilityElementProtocol]?

Returns the array of child accessibility elements in order for linear navigation.

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

