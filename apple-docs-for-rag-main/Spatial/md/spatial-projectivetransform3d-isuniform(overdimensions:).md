

- Spatial
- ProjectiveTransform3D
-  isUniform(overDimensions:) 

Instance Method

# isUniform(overDimensions:)

Returns a Boolean value that indicates whether the transform scales equally over the specified dimensions.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func isUniform(overDimensions: Dimension3DSet) -> Bool
```

## Parameters 

`overDimensions`  

The dimensions that the function checks over.

## See Also

### Checking characteristics

func is3DProjection() -> Bool

Returns a Boolean value that indicates whether the transform is a 3D projection.

var isAffine: Bool

A Boolean value that indicates whether the transform is affine.

var isIdentity: Bool

A Boolean value that indicates whether the transform is the identity transform.

var isRectilinear: Bool

A Boolean value that indicates whether the transform is rectilinear.

var isTranslation: Bool

A Boolean value that indicates whether the transform contains only a translation.

var isUniform: Bool

A Boolean value that indicates whether the transform scales equally over all dimensions.

var isInvertible: Bool

Returns a Boolean value that indicates whether the transform is invertible.

