

- AppKit
- NSPressGestureRecognizer
-  allowableMovement 

Instance Property

# allowableMovement

The maximum movement of the mouse in the view before the gesture fails.

macOS 10.10+

``` source
@MainActor
var allowableMovement: CGFloat { get set }
```

## Discussion

The mouse must move by the specified amount along either axis for the gesture to fail. The distance is measured in points. The default value of this property is the same as the double-click distance.

## See Also

### Configuring the Gesture Recognizer

var buttonMask: Int

A bit mask of the buttons required to recognize this press.

var minimumPressDuration: TimeInterval

The minimum time (in seconds) that the user must hold the mouse button in the view for a valid gesture.

var numberOfTouchesRequired: Int

The number of necessary touches on a Touch Bar for the gesture recognizer to match.

