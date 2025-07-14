

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
-  AnchoringComponent.Target.camera 

Case

# AnchoringComponent.Target.camera

An anchor point attached to the device’s camera.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
case camera
```

## See Also

### Basic anchor targets

case world(transform: float4x4)

An anchor point attached to a fixed position in the scene.

case plane(AnchoringComponent.Target.Alignment, classification: AnchoringComponent.Target.Classification, minimumBounds: SIMD2&lt;Float>)

An anchor point attached to a real world surface.

case anchor(identifier: UUID)

An anchor point attached to the AR anchor with a given identifier.

