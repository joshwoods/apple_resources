

- Model I/O
- MDLTransform
-  init(identity:) Deprecated

Initializer

# init(identity:)

Initializes a transform object to the identity transformation.

iOS 9.0–11.0DeprecatediPadOS 9.0–11.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.11–10.13DeprecatedtvOS 9.0–11.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
convenience init(identity: ())
```

## Return Value

A new transform object.

## Discussion

A transform matrix defines the local coordinate space transformations for a 3D object—that is, its position, orientation, shear, and scale. The identity transform is equivalent to no transformation, so an object affected by the transform uses the same coordinate space as its parent.

After initializing a transform object, you can use the translation, rotation, shear, and scale properties to individually work with those factors of the transform (or the corresponding methods listed in Using Factors of an Animated Transform to associate time-based transformation with each factor). To work with the complete transform matrix defined by those factors, use the matrix property.

## See Also

### Creating a Transform Object

convenience init(matrix: matrix_float4x4)

Initializes a transform object with the specified transform matrix.

convenience init(transformComponent: any MDLTransformComponent)

Initializes a transform object to match the specified transform component.

convenience init(matrix: matrix_float4x4, resetsTransform: Bool)

convenience init(transformComponent: any MDLTransformComponent, resetsTransform: Bool)

