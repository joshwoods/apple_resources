

- UIKit
- UIAccessibilityElement
-  accessibilityFrame 

Instance Property

# accessibilityFrame

The frame of the accessibility element, in screen coordinates.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var accessibilityFrame: CGRect { get set }
```

## Discussion

When you create an accessibility element to represent an element in your application, you must set this property to the `CGRect` structure that specifies the object’s screen location and size. (Objects that inherit from `UIView` include this information by default.)

Assigning a new value to this property changes the value of the accessibilityFrameInContainerSpace property to CGRectNull.

## See Also

### Related Documentation

static func convertToScreenCoordinates(CGRect, in: UIView) -> CGRect

Converts the specified rectangle from view coordinates to screen coordinates.

### Accessing the attributes of an accessibility element

var accessibilityLabel: String?

A string that succinctly identifies the accessibility element.

var accessibilityHint: String?

A string that briefly describes the result of performing an action on the accessibility element.

var accessibilityValue: String?

A string that represents the current value of the accessibility element.

var accessibilityFrameInContainerSpace: CGRect

The frame of the accessibility element, in the coordinate space of its container view.

var accessibilityTraits: UIAccessibilityTraits

The combination of traits that best characterize the accessibility element.

