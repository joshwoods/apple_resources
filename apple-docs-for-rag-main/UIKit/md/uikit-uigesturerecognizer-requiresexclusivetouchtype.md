

- UIKit
- UIGestureRecognizer
-  requiresExclusiveTouchType 

Instance Property

# requiresExclusiveTouchType

A Boolean value that indicates whether the gesture recognizer considers touches of different types simultaneously.

iOS 9.2+iPadOS 9.2+Mac Catalyst 13.1+tvOS 9.1+visionOS 1.0+

``` source
@MainActor
var requiresExclusiveTouchType: Bool { get set }
```

## Discussion

When the value of this property is true, the gesture recognizer automatically ignores new touches whose type doesn’t match the type of the initial touch. When the value is false, the gesture recognizer receives all touches whose types are listed in the allowedTouchTypes property.

## See Also

### Recognizing different gestures

var allowedPressTypes: [NSNumber]

An array of press types used to distinguish the type of button press.

var allowedTouchTypes: [NSNumber]

An array of touch types used to distinguish type of touches.

