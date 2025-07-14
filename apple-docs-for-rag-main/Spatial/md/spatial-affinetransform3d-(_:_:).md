

- Spatial
- AffineTransform3D
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Returns the concatenation of two affine transforms.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
static func * (lhs: AffineTransform3D, rhs: AffineTransform3D) -> AffineTransform3D
```

## Parameters 

`lhs`  

The left-hand-side value.

`rhs`  

The right-hand-side value.

## See Also

### Applying arithmetic operations

static func *= (inout AffineTransform3D, AffineTransform3D)

Concatenates two affine transforms and stores the result in the left-hand-side variable.

