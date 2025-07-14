

- AppKit
- NSPressGestureRecognizer
-  numberOfTouchesRequired 

Instance Property

# numberOfTouchesRequired

The number of necessary touches on a Touch Bar for the gesture recognizer to match.

macOS 10.12.2+

``` source
@MainActor
var numberOfTouchesRequired: Int { get set }
```

## See Also

### Related Documentation

class NSTouchBar

An object that provides dynamic contextual controls in the Touch Bar of supported models of MacBook Pro.

### Configuring the Gesture Recognizer

var allowableMovement: CGFloat

The maximum movement of the mouse in the view before the gesture fails.

var buttonMask: Int

A bit mask of the buttons required to recognize this press.

var minimumPressDuration: TimeInterval

The minimum time (in seconds) that the user must hold the mouse button in the view for a valid gesture.

