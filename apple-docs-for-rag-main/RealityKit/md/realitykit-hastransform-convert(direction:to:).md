

- RealityKit
- HasTransform
-  convert(direction:to:) 

Instance Method

# convert(direction:to:)

Converts a direction vector from the local space of the entity on which you called this method to the local space of a reference entity.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func convert(
    direction: SIMD3,
    to referenceEntity: Entity?
) -> SIMD3
```

## Parameters 

`direction`  

The direction vector given in the local space of the entity.

`referenceEntity`  

The entity that defines a frame of reference. Set this to `nil` to indicate world space.

## Return Value

The direction vector specified relative to `referenceEntity`.

## See Also

### Converting values between coordinate spaces

func convert(position: SIMD3&lt;Float>, from: Entity?) -> SIMD3&lt;Float>

Converts a position from the local space of a reference entity to the local space of the entity on which you called this method.

func convert(position: SIMD3&lt;Float>, to: Entity?) -> SIMD3&lt;Float>

Converts a position from the local space of the entity on which you called this method to the local space of a reference entity.

func convert(direction: SIMD3&lt;Float>, from: Entity?) -> SIMD3&lt;Float>

Converts a direction vector from the local space of a reference entity to the local space of the entity on which you called this method.

func convert(normal: SIMD3&lt;Float>, from: Entity?) -> SIMD3&lt;Float>

Converts a normal vector from the local space of a reference entity to the local space of the entity on which you called this method.

func convert(normal: SIMD3&lt;Float>, to: Entity?) -> SIMD3&lt;Float>

Converts a normal vector from the local space of the entity on which you called this method to the local space of a reference entity.

func convert(transform: Transform, from: Entity?) -> Transform

Converts the scale, rotation, and position of a transform from the local space of a reference entity to the local space of the entity on which you called this method.

func convert(transform: Transform, to: Entity?) -> Transform

Converts the scale, rotation, and position of a transform from the local space of the entity on which you called this method to the local space of a reference entity.

