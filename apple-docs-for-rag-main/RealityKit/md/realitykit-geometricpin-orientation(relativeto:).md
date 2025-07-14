

- RealityKit
- GeometricPin
-  orientation(relativeTo:) 

Instance Method

# orientation(relativeTo:)

Calculates and returns the current orientation of the pin relative to a reference entity, adjusted by the optional offset position.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
@MainActor
func orientation(relativeTo referenceEntity: Entity?) -> simd_quatf?
```

## Parameters 

`referenceEntity`  

Reference `Entity` which defines the frame of reference for the returned orientation. Can be `nil`, which is equivalent to “world space”.

