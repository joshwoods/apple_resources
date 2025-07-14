

- UIKit
- UIAccessibilityElement
-  accessibilityValue 

Instance Property

# accessibilityValue

A string that represents the current value of the accessibility element.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var accessibilityValue: String? { get set }
```

## Discussion

The value is a localized string that contains the current value of an element. For example, the value of a slider might be 9.5 or 35% and the value of a text field is the text it contains.

Use the value property only when an accessibility element can have a value that is not represented by its label. For example, a volume slider’s label might be “Volume,” but its value is the current volume level. In this case, it’s not enough for users to know the identity of the slider, because they also need to know its current value. The label of a Save button, on the other hand, tells users everything they need to know about the control; supplying the word “Save” as a value would be unnecessary and confusing.

## See Also

### Accessing the attributes of an accessibility element

var accessibilityLabel: String?

A string that succinctly identifies the accessibility element.

var accessibilityHint: String?

A string that briefly describes the result of performing an action on the accessibility element.

var accessibilityFrame: CGRect

The frame of the accessibility element, in screen coordinates.

var accessibilityFrameInContainerSpace: CGRect

The frame of the accessibility element, in the coordinate space of its container view.

var accessibilityTraits: UIAccessibilityTraits

The combination of traits that best characterize the accessibility element.

