

- UIKit
- UILongPressGestureRecognizer
-  minimumPressDuration 

Instance Property

# minimumPressDuration

The minimum time that the user must press on the view for the gesture to be recognized.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var minimumPressDuration: TimeInterval { get set }
```

## Mentioned in 

Handling long-press gestures

## Discussion

The time interval is in seconds. The default duration is `0.5` seconds.

## See Also

### Configuring the gesture recognizer

var numberOfTouchesRequired: Int

The number of fingers that must touch the view for gesture recognition.

var numberOfTapsRequired: Int

The number of taps on the view necessary for gesture recognition.

var allowableMovement: CGFloat

The maximum movement of the fingers on the view before the gesture fails.

