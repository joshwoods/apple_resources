

- Spatial
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Returns the rotatable entity that results from applying the rotatable entity.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func * (lhs: Rotation3D, rhs: T) -> T where T : Rotatable3D
```

## Parameters 

`lhs`  

The left-hand-side value.

`rhs`  

The right-hand-side value.

## See Also

### Applying arithmetic operations

static func * (Rotation3D, Rotation3D) -> Rotation3D

Returns the product of two rotations.

static func * (Rotation3D, Double) -> Rotation3D

Returns the spherical linear interpolation between the identity rotation and the left-hand-side rotation at the right-hand-side interpolation parameter.

static func * (Double, Rotation3D) -> Rotation3D

Returns the spherical linear interpolation between the identity rotation and the right-hand-side rotation at the left-hand-side interpolation parameter.

static func *= (inout Rotation3D, Rotation3D)

Computes the product of two rotations and stores the result in the left-hand-side variable.

