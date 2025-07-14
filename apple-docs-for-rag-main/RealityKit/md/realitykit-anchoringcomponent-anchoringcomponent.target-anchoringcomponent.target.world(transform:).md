

- RealityKit
- AnchoringComponent
- AnchoringComponent.Target
-  AnchoringComponent.Target.world(transform:) 

Case

# AnchoringComponent.Target.world(transform:)

An anchor point attached to a fixed position in the scene.

iOS 13.0+iPadOS 13.0+Mac Catalyst 14.0+macOS 10.15+visionOS

``` source
case world(transform: float4x4)
```

## See Also

### Basic anchor targets

case plane(AnchoringComponent.Target.Alignment, classification: AnchoringComponent.Target.Classification, minimumBounds: SIMD2&lt;Float>)

An anchor point attached to a real world surface.

case camera

An anchor point attached to the device’s camera.

case anchor(identifier: UUID)

An anchor point attached to the AR anchor with a given identifier.

