

- UIKit
- UIGestureRecognizer
-  allowedPressTypes 

Instance Property

# allowedPressTypes

An array of press types used to distinguish the type of button press.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var allowedPressTypes: [NSNumber] { get set }
```

## Discussion

This property is an array of `UIPressTypes` that activates the gesture recognizer to distinguish the type of button press. The default press type is UIPress.PressType.select. When this property is set to an empty array, the gesture recognizer will respond to taps like a touch pad like surface. For a list of possible press types, see UIPress.PressType enumeration in the UIPress.

## See Also

### Recognizing different gestures

var allowedTouchTypes: [NSNumber]

An array of touch types used to distinguish type of touches.

var requiresExclusiveTouchType: Bool

A Boolean value that indicates whether the gesture recognizer considers touches of different types simultaneously.

