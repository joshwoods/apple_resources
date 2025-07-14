

- UIKit
- UIRotationGestureRecognizer
-  rotation 

Instance Property

# rotation

The rotation of the gesture in radians.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var rotation: CGFloat { get set }
```

## Mentioned in 

Handling rotation gestures

## Discussion

You may set the rotation value to an arbitrary value; however, setting the rotation resets the velocity.

The rotation value is a single value that varies over time. It isn’t the delta value from the last time that the rotation was reported. Apply the rotation value to the state of the view when the gesture is first recognized — don’t concatenate the value each time the handler is called.

## See Also

### Interpreting the gesture

var velocity: CGFloat

The velocity of the rotation gesture in radians per second.

