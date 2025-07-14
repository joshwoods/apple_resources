

- UIKit
- UIGestureRecognizer
-  allowedTouchTypes 

Instance Property

# allowedTouchTypes

An array of touch types used to distinguish type of touches.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var allowedTouchTypes: [NSNumber] { get set }
```

## Discussion

This property is an array of touch types that recognizes whether the touch is direct or indirect. For a list of all possible touch types, see UITouch.TouchType enumeration in UITouch. The default value of this property contains all touch types.

## See Also

### Recognizing different gestures

var allowedPressTypes: [NSNumber]

An array of press types used to distinguish the type of button press.

var requiresExclusiveTouchType: Bool

A Boolean value that indicates whether the gesture recognizer considers touches of different types simultaneously.

