

- Spatial
- Pose3D
-  \*=(\_:\_:) 

Operator

# \*=(\_:\_:)

Concatenates two poses and stores the result in the left-hand-side variable.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func *= (lhs: inout Pose3D, rhs: Pose3D)
```

## Parameters 

`lhs`  

The left-hand-side value.

`rhs`  

The right-hand-side value.

## See Also

### Applying arithmetic operations

static func * (Pose3D, Pose3D) -> Pose3D

Returns the concatenation of two poses.

