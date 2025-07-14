

- AppKit
- NSAccessibilityLayoutArea
-  accessibilitySelectedChildren() 

Instance Method

# accessibilitySelectedChildren()

Returns the layout area’s currently selected children.

macOS

``` source
func accessibilitySelectedChildren() -> [Any]?
```

**Required**

## Return Value

An array containing the currently selected children. If no children are selected, this method returns an empty array.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilitySelectedChildren property.

## See Also

### Supporting Accessibility

func accessibilityChildren() -> [Any]?

Returns the accessibility element’s children in the accessibility hierarchy.

**Required**

var accessibilityFocusedUIElement: Any

The child accessibility element with the current focus.

**Required**

func accessibilityLabel() -> String

Returns a short description of the layout area.

**Required**

