

- RealityKit
- EntityRotationGestureRecognizer
-  touchesBegan(\_:with:) 

Instance Method

# touchesBegan(\_:with:)

Sent to the gesture recognizer when one or more fingers touch down on the associated entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
@MainActor @preconcurrency
override dynamic func touchesBegan(
    _ touches: Set,
    with event: UIEvent
)
```

## Parameters 

`touches`  

A set of `UITouch` instances in the event represented by `event` that represent the touches in the `UITouch.Phase.began` phase.

`event`  

A `UIEvent` object representing the event to which the touches belong.

## See Also

### Using the recognizer

var entity: (any HasCollision)?

The entity the receiver is associated with

func canPrevent(UIGestureRecognizer) -> Bool

