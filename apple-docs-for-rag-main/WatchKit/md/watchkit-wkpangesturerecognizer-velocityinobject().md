

- WatchKit
- WKPanGestureRecognizer
-  velocityInObject() 

Instance Method

# velocityInObject()

The velocity of the pan gesture in the current object.

watchOS 3.0+

``` source
func velocityInObject() -> CGPoint
```

## Return Value

The velocity of the gesture, which is expressed in points per second. The `x` field contains the horizontal velocity and the `y` field contains the vertical velocity.

## See Also

### Tracking the Location and Velocity of the Gesture

func translationInObject() -> CGPoint

The amount of translation for the pan gesture in the current object.

