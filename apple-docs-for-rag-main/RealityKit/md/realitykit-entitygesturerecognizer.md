

- RealityKit
-  EntityGestureRecognizer 

Protocol

# EntityGestureRecognizer

A gesture recognizer that works on entities.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
protocol EntityGestureRecognizer : UIGestureRecognizer
```

## Topics

### Using the gesture recognizer

var entity: (any HasCollision)?

The entity the receiver is associated with

**Required**

func location(in: Entity?) -> SIMD3&lt;Float>?

Returns the unprojected location of the gesture represented by the receiver in the space of the given entity.

**Required** Default implementation provided.

## Relationships

### Inherits From

- UIGestureRecognizer

### Conforming Types

- EntityRotationGestureRecognizer
- EntityScaleGestureRecognizer
- EntityTranslationGestureRecognizer

## See Also

### UIKit and AppKit gestures

struct EntityGestures

The set of possible entity gesture recognizers.

class EntityRotationGestureRecognizer

A gesture recognizer that uses rotation gestures involving two touches to rotate a given entity.

class EntityScaleGestureRecognizer

A gesture recognizer that uses a pinch gesture to scale or zoom an entity.

class EntityTranslationGestureRecognizer

A gesture recognizer that uses a pan gesture to move an entity.

