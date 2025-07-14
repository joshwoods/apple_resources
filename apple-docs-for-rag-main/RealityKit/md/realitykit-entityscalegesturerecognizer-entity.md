

- RealityKit
- EntityScaleGestureRecognizer
-  entity 

Instance Property

# entity

The entity the receiver is associated with

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
@MainActor @preconcurrency
var entity: (any HasCollision)? { get set }
```

## See Also

### Using the recognizer

func canPrevent(UIGestureRecognizer) -> Bool

func touchesBegan(Set&lt;UITouch>, with: UIEvent)

Sent to the gesture recognizer when one or more fingers touch down on the associated entity.

