

- Spatial
- ProjectiveTransform3D
-  isInvertible 

Instance Property

# isInvertible

Returns a Boolean value that indicates whether the transform is invertible.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
var isInvertible: Bool { get }
```

## See Also

### Checking characteristics

func is3DProjection() -> Bool

Returns a Boolean value that indicates whether the transform is a 3D projection.

func isUniform(overDimensions: Dimension3DSet) -> Bool

Returns a Boolean value that indicates whether the transform scales equally over the specified dimensions.

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

