

- Compositor Services
- LayerRenderer
-  onSpatialEvent 

Instance Property

# onSpatialEvent

A closure that receives spatial event updates from the layer renderer.

CompositorServicesSwiftUIvisionOS 1.0+

``` source
@MainActor @preconcurrency
var onSpatialEvent: @MainActor (SpatialEventCollection) -> Void { get set }
```

## Discussion

Assign a closure to this property when configuring your layer renderer. When a person interacts with your immersive content, the layer renderer delivers the associated events as a parameter to your closure.

