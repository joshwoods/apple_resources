

- Spatial
- Rotation3D
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Returns the spherical linear interpolation between the identity rotation and the right-hand-side rotation at the left-hand-side interpolation parameter.

iOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
static func * (lhs: Double, rhs: Rotation3D) -> Rotation3D
```

## Parameters 

`lhs`  

The interpolation parameter.

`rhs`  

The rotation.

## See Also

### Applying arithmetic operations

static func * (Rotation3D, Rotation3D) -> Rotation3D

Returns the product of two rotations.

static func * (Rotation3D, Double) -> Rotation3D

Returns the spherical linear interpolation between the identity rotation and the left-hand-side rotation at the right-hand-side interpolation parameter.

func * &lt;T>(Rotation3D, T) -> T

Returns the rotatable entity that results from applying the rotatable entity.

static func *= (inout Rotation3D, Rotation3D)

Computes the product of two rotations and stores the result in the left-hand-side variable.

