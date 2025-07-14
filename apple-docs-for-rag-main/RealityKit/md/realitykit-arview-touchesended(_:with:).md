

- RealityKit
- ARView
-  touchesEnded(\_:with:) 

Instance Method

# touchesEnded(\_:with:)

Tells the view when one or more fingers are raised from the view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+

``` source
@MainActor @preconcurrency
override dynamic func touchesEnded(
    _ touches: Set,
    with event: UIEvent?
)
```

## Parameters 

`touches`  

A set of `UITouch` instances that represent the touches whose values changed. These touches all belong to the specified `event`. For touches in a view, this set contains only one touch by default. To receive multiple touches, set the view’s isMultipleTouchEnabled property to `true`.

`event`  

The event to which the touches belong.

## Discussion

See touchesEnded(_:with:) for more information.

## See Also

### Handling touch input

func touchesBegan(Set&lt;UITouch>, with: UIEvent?)

Tells the view that one or more new touches occurred.

func touchesMoved(Set&lt;UITouch>, with: UIEvent?)

Tells the view when one or more touches associated with an event changed.

func touchesCancelled(Set&lt;UITouch>, with: UIEvent?)

Tells the view when a system event (such as a system alert) cancels a touch sequence.

