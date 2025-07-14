

- UIKit
- UIAccessibilityElement
-  accessibilityLabel 

Instance Property

# accessibilityLabel

A string that succinctly identifies the accessibility element.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var accessibilityLabel: String? { get set }
```

## Mentioned in 

Supporting VoiceOver in your app

## Discussion

The label is a very short, localized string that identifies the accessibility element, but does not include the type of the control or view. For example, the label for a Save button is “Save,” not “Save button.”

By default, standard UIKit controls and views have labels that derive from their titles. If you provide a custom control or view, however, you need to set this property appropriately so that assistive applications can supply accurate information to users with disabilities.

## See Also

### Accessing the attributes of an accessibility element

var accessibilityHint: String?

A string that briefly describes the result of performing an action on the accessibility element.

var accessibilityValue: String?

A string that represents the current value of the accessibility element.

var accessibilityFrame: CGRect

The frame of the accessibility element, in screen coordinates.

var accessibilityFrameInContainerSpace: CGRect

The frame of the accessibility element, in the coordinate space of its container view.

var accessibilityTraits: UIAccessibilityTraits

The combination of traits that best characterize the accessibility element.

