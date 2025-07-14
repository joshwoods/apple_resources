

- RealityKit
- ARView
-  gestureRecognizer(\_:shouldRecognizeSimultaneouslyWith:) 

Instance Method

# gestureRecognizer(\_:shouldRecognizeSimultaneouslyWith:)

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
@MainActor @preconcurrency @objc
dynamic func gestureRecognizer(
    _ gestureRecognizer: UIGestureRecognizer,
    shouldRecognizeSimultaneouslyWith otherGestureRecognizer: UIGestureRecognizer
) -> Bool
```

## See Also

### Adding gesture recognizers to entities

func installGestures(ARView.EntityGestures, for: any HasCollision) -> [any EntityGestureRecognizer]

Installs standard gestures onto the given entity, configured to be recognized simultaneously.

