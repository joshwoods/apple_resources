

- UIKit
- UILongPressGestureRecognizer
-  numberOfTouchesRequired 

Instance Property

# numberOfTouchesRequired

The number of fingers that must touch the view for gesture recognition.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var numberOfTouchesRequired: Int { get set }
```

## Mentioned in 

Handling long-press gestures

## Discussion

The default number of fingers is `1`.

## See Also

### Configuring the gesture recognizer

var minimumPressDuration: TimeInterval

The minimum time that the user must press on the view for the gesture to be recognized.

var numberOfTapsRequired: Int

The number of taps on the view necessary for gesture recognition.

var allowableMovement: CGFloat

The maximum movement of the fingers on the view before the gesture fails.

