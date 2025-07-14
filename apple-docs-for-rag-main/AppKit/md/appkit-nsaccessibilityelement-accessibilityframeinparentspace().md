

- AppKit
- NSAccessibilityElement
-  accessibilityFrameInParentSpace() 

Instance Method

# accessibilityFrameInParentSpace()

Returns the accessibility element’s frame in its parent’s coordinate system.

macOS 10.10+

``` source
func accessibilityFrameInParentSpace() -> NSRect
```

## See Also

### Supporting the Accessibility Hierarchy

class func element(withRole: NSAccessibility.Role, frame: NSRect, label: String?, parent: Any?) -> Any

Instantiates and configures a new accessibility element.

func accessibilityAddChildElement(NSAccessibilityElement)

Adds a child to the accessibility element in the accessibility hierarchy.

func setAccessibilityFrameInParentSpace(NSRect)

Sets the accessibility element’s frame in its parent’s coordinate system.

