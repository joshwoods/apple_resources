

- UIKit
- UILongPressGestureRecognizer
-  numberOfTapsRequired 

Instance Property

# numberOfTapsRequired

The number of taps on the view necessary for gesture recognition.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var numberOfTapsRequired: Int { get set }
```

## Mentioned in 

Handling long-press gestures

## Discussion

The default number of taps is `0`.

## See Also

### Configuring the gesture recognizer

var minimumPressDuration: TimeInterval

The minimum time that the user must press on the view for the gesture to be recognized.

var numberOfTouchesRequired: Int

The number of fingers that must touch the view for gesture recognition.

var allowableMovement: CGFloat

The maximum movement of the fingers on the view before the gesture fails.

