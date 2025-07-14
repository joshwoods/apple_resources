

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
-  AnchoringComponent.Target.anchor(identifier:) 

Case

# AnchoringComponent.Target.anchor(identifier:)

An anchor point attached to the AR anchor with a given identifier.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+

``` source
case anchor(identifier: UUID)
```

## See Also

### Basic anchor targets

case world(transform: float4x4)

An anchor point attached to a fixed position in the scene.

case plane(AnchoringComponent.Target.Alignment, classification: AnchoringComponent.Target.Classification, minimumBounds: SIMD2&lt;Float>)

An anchor point attached to a real world surface.

case camera

An anchor point attached to the device’s camera.

