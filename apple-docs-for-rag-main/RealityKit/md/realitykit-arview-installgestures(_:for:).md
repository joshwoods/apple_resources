

- RealityKit
- ARView
-  installGestures(\_:for:) 

Instance Method

# installGestures(\_:for:)

Installs standard gestures onto the given entity, configured to be recognized simultaneously.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+

``` source
@discardableResult @MainActor @preconcurrency
func installGestures(
    _ gestures: ARView.EntityGestures = .all,
    for entity: any HasCollision
) -> [any EntityGestureRecognizer]
```

## Parameters 

`gestures`  

The gesture types to install.

`entity`  

The entity with which to associate the gesture recognizers.

## Return Value

The set of gesture recognizers created to handle the requested gestures.

## See Also

### Adding gesture recognizers to entities

func gestureRecognizer(UIGestureRecognizer, shouldRecognizeSimultaneouslyWith: UIGestureRecognizer) -> Bool

