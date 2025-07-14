

- RealityKit
- EntityTranslationGestureRecognizer
-  reset() 

Instance Method

# reset()

Overridden to reset internal state when a gesture recognition attempt completes.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
@MainActor @preconcurrency
override dynamic func reset()
```

## See Also

### Using the recognizer

var entity: (any HasCollision)?

The entity the receiver is associated with

func canPrevent(UIGestureRecognizer) -> Bool

func location(in: Entity?) -> SIMD3&lt;Float>?

Returns the unprojected location of the gesture represented by the receiver in the space of the given entity.

func setTranslation(SIMD3&lt;Float>, in: Entity?)

Sets the translation of the receiver in the entity’s coordinate space

func touchesBegan(Set&lt;UITouch>, with: UIEvent)

Sent to the gesture recognizer when one or more fingers touch down on the associated entity.

func touchesCancelled(Set&lt;UITouch>, with: UIEvent)

Sent to the gesture recognizer when a system event (such as an incoming phone call) cancels a touch event.

func touchesEnded(Set&lt;UITouch>, with: UIEvent)

Sent to the gesture recognizer when one or more fingers lift from the associated view.

func touchesMoved(Set&lt;UITouch>, with: UIEvent)

Sent to the gesture recognizer when one or more fingers move in the associated view.

func translation(in: Entity?) -> SIMD3&lt;Float>?

The translation of the gesture in the space of the specified entity.

func velocity(in: Entity?) -> SIMD3&lt;Float>

The velocity of the translation gesture in the space of the specified entity.

