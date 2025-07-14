

- AppKit
- NSAccessibilityLayoutArea
-  accessibilityChildren() 

Instance Method

# accessibilityChildren()

Returns the accessibility element’s children in the accessibility hierarchy.

macOS

``` source
func accessibilityChildren() -> [Any]?
```

**Required**

## Return Value

An array that contains references to this element’s children in the accessibility hierarchy.

## Discussion

This method is the getter for the NSAccessibilityProtocol protocol’s accessibilityChildren property.

## See Also

### Related Documentation

func accessibilityAddChildElement(NSAccessibilityElement)

Adds a child to the accessibility element in the accessibility hierarchy.

static func unignoredChildrenForOnlyChild(from: Any) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

static func unignoredChildren(from: [Any]) -> [Any]

Returns a list of unignored accessibility objects, descending the hierarchy, if necessary.

### Supporting Accessibility

var accessibilityFocusedUIElement: Any

The child accessibility element with the current focus.

**Required**

func accessibilityLabel() -> String

Returns a short description of the layout area.

**Required**

func accessibilitySelectedChildren() -> [Any]?

Returns the layout area’s currently selected children.

**Required**

