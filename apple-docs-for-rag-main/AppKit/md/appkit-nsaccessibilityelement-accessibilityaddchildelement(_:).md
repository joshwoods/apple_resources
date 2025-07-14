

- AppKit
- NSAccessibilityElement
-  accessibilityAddChildElement(\_:) 

Instance Method

# accessibilityAddChildElement(\_:)

Adds a child to the accessibility element in the accessibility hierarchy.

macOS 10.10+

``` source
func accessibilityAddChildElement(_ childElement: NSAccessibilityElement)
```

## Parameters 

`childElement`  

The child element to be added.

## Discussion

Calling this method sets up the proper parent-child relationship between the current element and the provided child element.

## See Also

### Supporting the Accessibility Hierarchy

class func element(withRole: NSAccessibility.Role, frame: NSRect, label: String?, parent: Any?) -> Any

Instantiates and configures a new accessibility element.

func accessibilityFrameInParentSpace() -> NSRect

Returns the accessibility element’s frame in its parent’s coordinate system.

func setAccessibilityFrameInParentSpace(NSRect)

Sets the accessibility element’s frame in its parent’s coordinate system.

