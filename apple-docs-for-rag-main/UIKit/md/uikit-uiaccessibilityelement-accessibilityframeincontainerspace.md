

- UIKit
- UIAccessibilityElement
-  accessibilityFrameInContainerSpace 

Instance Property

# accessibilityFrameInContainerSpace

The frame of the accessibility element, in the coordinate space of its container view.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
var accessibilityFrameInContainerSpace: CGRect { get set }
```

## Discussion

The default value of this property is CGRectNull. Use this property to set the frame rectangle of an element whose frame rectangle could be affected by its container view. For example, use this property to set the frame rectangle for an element in a scroll view’s content view. Changing the value of this property automatically adjusts the rectangle in the accessibilityFrame property.

## See Also

### Accessing the attributes of an accessibility element

var accessibilityLabel: String?

A string that succinctly identifies the accessibility element.

var accessibilityHint: String?

A string that briefly describes the result of performing an action on the accessibility element.

var accessibilityValue: String?

A string that represents the current value of the accessibility element.

var accessibilityFrame: CGRect

The frame of the accessibility element, in screen coordinates.

var accessibilityTraits: UIAccessibilityTraits

The combination of traits that best characterize the accessibility element.

