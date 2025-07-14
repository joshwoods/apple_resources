

- RealityKit
-  EntityScaleGestureRecognizer 

Class

# EntityScaleGestureRecognizer

A gesture recognizer that uses a pinch gesture to scale or zoom an entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
@MainActor @objc @preconcurrency
class EntityScaleGestureRecognizer
```

## Topics

### Creating the recognizer

init(target: Any?, action: Selector?)

### Using the recognizer

var entity: (any HasCollision)?

The entity the receiver is associated with

func canPrevent(UIGestureRecognizer) -> Bool

func touchesBegan(Set&lt;UITouch>, with: UIEvent)

Sent to the gesture recognizer when one or more fingers touch down on the associated entity.

## Relationships

### Inherits From

- UIPinchGestureRecognizer

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

class EntityTranslationGestureRecognizer

A gesture recognizer that uses a pan gesture to move an entity.

protocol EntityGestureRecognizer

A gesture recognizer that works on entities.

