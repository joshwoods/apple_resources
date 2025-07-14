

- UIKit
- UIAccessibilityElement
-  accessibilityTraits 

Instance Property

# accessibilityTraits

The combination of traits that best characterize the accessibility element.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var accessibilityTraits: UIAccessibilityTraits { get set }
```

## Discussion

A trait describes a single aspect of an element’s behavior, state, or usage. Several traits are combined in this property (using an OR operation) to give a complete picture of the element to an assistive application. See “Accessibility Traits” in UIAccessibility for a complete list of traits.

UIKit provides an appropriate combination of traits for all standard controls and views. When combining traits for a custom accessibility element, be sure to:

- Use common sense. Don’t combine traits that characterize the element in mutually exclusive ways, such as combining the button and search-field traits.

- Combine the traits you select with the superclass’s traits. Specifically, always combine your custom traits with `[super accessibilityTraits]` in the method you use to set a custom element’s traits.

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

var accessibilityFrameInContainerSpace: CGRect

The frame of the accessibility element, in the coordinate space of its container view.

