

- AppKit
- NSAccessibilityLayoutArea
-  accessibilityFocusedUIElement 

Instance Property

# accessibilityFocusedUIElement

The child accessibility element with the current focus.

macOS

``` source
var accessibilityFocusedUIElement: Any { get }
```

**Required**

## See Also

### Supporting Accessibility

func accessibilityChildren() -> [Any]?

Returns the accessibility element’s children in the accessibility hierarchy.

**Required**

func accessibilityLabel() -> String

Returns a short description of the layout area.

**Required**

func accessibilitySelectedChildren() -> [Any]?

Returns the layout area’s currently selected children.

**Required**

