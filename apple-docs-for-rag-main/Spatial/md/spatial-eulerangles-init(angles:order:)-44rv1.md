

- Spatial
- EulerAngles
-  init(angles:order:) 

Initializer

# init(angles:order:)

Creates a new Euler angles structure from the specified single-precision angles and order.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    angles: simd_float3,
    order: EulerAngles.Order
)
```

## Parameters 

`angles`  

A three-element, single-precision vector that specifies the Euler angles.

`order`  

The Euler angle order.

## See Also

### Initializers

init()

Creates a new Euler angles structure.

init(angles: simd_double3, order: __SPEulerAngleOrder)

Creates a new Euler angles structure from the specified double-precision angles and order.

init(x: Angle2D, y: Angle2D, z: Angle2D, order: EulerAngles.Order)

Creates a new Euler angles structure from the specified angle structures and order.

init(Angle2D, Angle2D, Angle2D, order: EulerAngles.Order)

Creates a new Euler angles structure from the specified angle structures and order.

Deprecated

