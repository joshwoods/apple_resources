

- RealityKit
- BindTarget
- BindTarget.EntityPath
-  self 

Instance Property

# self

A bind target for the entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var `self`: BindTarget { get }
```

## Discussion

This property represents a bind path within an AnimationView to redirect the view’s source animation to a different scene.

## See Also

### Accessing a bind target

var jointTransforms: BindTarget

A bind target for the entity’s joint transforms.

var transform: BindTarget

A bind target for the entity’s transform.

func parameter(String) -> BindTarget

Provides a bind target for a particular animated property.

