

- AppKit
- NSAccessibilityElement
-  setAccessibilityFrameInParentSpace(\_:) 

Instance Method

# setAccessibilityFrameInParentSpace(\_:)

Sets the accessibility element’s frame in its parent’s coordinate system.

macOS 10.10+

``` source
func setAccessibilityFrameInParentSpace(_ accessibilityFrameInParentSpace: NSRect)
```

## See Also

### Supporting the Accessibility Hierarchy

class func element(withRole: NSAccessibility.Role, frame: NSRect, label: String?, parent: Any?) -> Any

Instantiates and configures a new accessibility element.

func accessibilityAddChildElement(NSAccessibilityElement)

Adds a child to the accessibility element in the accessibility hierarchy.

func accessibilityFrameInParentSpace() -> NSRect

Returns the accessibility element’s frame in its parent’s coordinate system.

