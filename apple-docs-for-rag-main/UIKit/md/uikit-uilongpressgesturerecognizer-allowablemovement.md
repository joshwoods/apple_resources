

- UIKit
- UILongPressGestureRecognizer
-  allowableMovement 

Instance Property

# allowableMovement

The maximum movement of the fingers on the view before the gesture fails.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var allowableMovement: CGFloat { get set }
```

## Discussion

The allowable distance, measured in points. The default distance is `10` points.

## See Also

### Configuring the gesture recognizer

var minimumPressDuration: TimeInterval

The minimum time that the user must press on the view for the gesture to be recognized.

var numberOfTouchesRequired: Int

The number of fingers that must touch the view for gesture recognition.

var numberOfTapsRequired: Int

The number of taps on the view necessary for gesture recognition.

