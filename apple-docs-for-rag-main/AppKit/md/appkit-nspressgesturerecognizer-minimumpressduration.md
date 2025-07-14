

- AppKit
- NSPressGestureRecognizer
-  minimumPressDuration 

Instance Property

# minimumPressDuration

The minimum time (in seconds) that the user must hold the mouse button in the view for a valid gesture.

macOS 10.10+

``` source
@MainActor
var minimumPressDuration: TimeInterval { get set }
```

## Discussion

The default value of this property is the same as the current double-click interval.

## See Also

### Configuring the Gesture Recognizer

var allowableMovement: CGFloat

The maximum movement of the mouse in the view before the gesture fails.

var buttonMask: Int

A bit mask of the buttons required to recognize this press.

var numberOfTouchesRequired: Int

The number of necessary touches on a Touch Bar for the gesture recognizer to match.

