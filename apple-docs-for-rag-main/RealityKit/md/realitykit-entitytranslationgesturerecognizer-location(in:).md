

- RealityKit
- EntityTranslationGestureRecognizer
-  location(in:) 

Instance Method

# location(in:)

Returns the unprojected location of the gesture represented by the receiver in the space of the given entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
@MainActor @preconcurrency
func location(in entity: Entity?) -> SIMD3?
```

## Parameters 

`entity`  

An entity in whose space the location is computed. A `nil` entity will result in world space.

## Return Value

The 3D position identifying the location of the gesture in the space specified.

## Discussion

The location is typically the result of a centroid of touches for a gesture, unprojected onto the associated `entity`, and then converted into the space of the entity passed in, or world space if `nil` is passed in.

## See Also

### Using the recognizer

var entity: (any HasCollision)?

The entity the receiver is associated with

func canPrevent(UIGestureRecognizer) -> Bool

func reset()

Overridden to reset internal state when a gesture recognition attempt completes.

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

