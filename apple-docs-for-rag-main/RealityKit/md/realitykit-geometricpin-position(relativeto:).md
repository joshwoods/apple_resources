

- RealityKit
- GeometricPin
-  position(relativeTo:) 

Instance Method

# position(relativeTo:)

Calculates and returns the current position of the pin relative to a reference entity, adjusted by the optional offset position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
func position(relativeTo referenceEntity: Entity?) -> SIMD3?
```

## Parameters 

`referenceEntity`  

Reference `Entity` which defines the frame of reference for the returned position. Can be `nil`, which is equivalent to “world space”.

