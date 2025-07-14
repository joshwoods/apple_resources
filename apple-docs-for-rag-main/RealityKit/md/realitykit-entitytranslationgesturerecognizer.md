

- RealityKit
-  EntityTranslationGestureRecognizer 

Class

# EntityTranslationGestureRecognizer

A gesture recognizer that uses a pan gesture to move an entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
@MainActor @objc @preconcurrency
class EntityTranslationGestureRecognizer
```

## Overview

A gesture recognizer that handles pan and dragging gestures on an entity.

## Topics

### Creating a recognizer

init(target: Any?, action: Selector?)

### Using the recognizer

var entity: (any HasCollision)?

The entity the receiver is associated with

func canPrevent(UIGestureRecognizer) -> Bool

func location(in: Entity?) -> SIMD3&lt;Float>?

Returns the unprojected location of the gesture represented by the receiver in the space of the given entity.

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

### Default Implementations

EntityGestureRecognizer Implementations

## Relationships

### Inherits From

- UIGestureRecognizer

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- EntityGestureRecognizer
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### UIKit and AppKit gestures

struct EntityGestures

The set of possible entity gesture recognizers.

class EntityRotationGestureRecognizer

A gesture recognizer that uses rotation gestures involving two touches to rotate a given entity.

class EntityScaleGestureRecognizer

A gesture recognizer that uses a pinch gesture to scale or zoom an entity.

protocol EntityGestureRecognizer

A gesture recognizer that works on entities.

