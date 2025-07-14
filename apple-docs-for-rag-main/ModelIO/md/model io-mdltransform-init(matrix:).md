

- Model I/O
- MDLTransform
-  init(matrix:) 

Initializer

# init(matrix:)

Initializes a transform object with the specified transform matrix.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(matrix: matrix_float4x4)
```

## Parameters 

`matrix`  

A transform matrix that defines a local coordinate space relative to a parent coordinate space.

## Return Value

A new transform object.

## Discussion

A transform matrix defines the local coordinate space transformations for a 3D object—that is, its position, orientation, shear, and scale.

After initializing a transform object from a matrix, you can use the translation, rotation, shear, and scale properties to individually work with those factors of the transform (or the corresponding methods listed in Using Factors of an Animated Transform to associate time-based transformation with each factor). To work with the complete transform matrix defined by those factors, use the matrix property.

The `matrix` parameter must be an invertible, homogeneous affine transform matrix. If you initialize a transform object with a nonaffine transform matrix, attempts to retrieve its translation, rotation, shear, or scale factors instead return identity values.

## See Also

### Creating a Transform Object

convenience init(identity: ())

Initializes a transform object to the identity transformation.

Deprecated

convenience init(transformComponent: any MDLTransformComponent)

Initializes a transform object to match the specified transform component.

convenience init(matrix: matrix_float4x4, resetsTransform: Bool)

convenience init(transformComponent: any MDLTransformComponent, resetsTransform: Bool)

