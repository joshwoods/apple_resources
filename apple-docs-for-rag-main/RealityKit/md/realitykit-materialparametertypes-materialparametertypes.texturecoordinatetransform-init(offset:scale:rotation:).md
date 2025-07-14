

- RealityKit
- MaterialParameterTypes
- MaterialParameterTypes.TextureCoordinateTransform
-  init(offset:scale:rotation:) 

Initializer

# init(offset:scale:rotation:)

Creates a texture coordinate transform object.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
init(
    offset: SIMD2 = .init(),
    scale: SIMD2 = .init(1, 1),
    rotation: Float = 0.0
)
```

## Parameters 

`offset`  

The amount to offset the UV texture coordinates.

`scale`  

The amount to scale the UV texture coordinates.

`rotation`  

The amount to rotate the UV texture coordinates in radians.

