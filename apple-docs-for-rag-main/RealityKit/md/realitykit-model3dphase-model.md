

- RealityKit
- Model3DPhase
-  model 

Instance Property

# model

The loaded model, if any.

RealityKitSwiftUIvisionOS 1.0+

``` source
var model: ResolvedModel3D? { get }
```

## Discussion

If this value isn’t `nil`, the model load operation has finished, and you can use the model to update the view. You can use the model directly, or you can modify it in some way. For example, you can add a `ResolvedModel3D/resizable()` modifier to make the model resizable.

## See Also

### Accessing the model

var error: (any Error)?

The error that occurred when attempting to load a model, if any.

