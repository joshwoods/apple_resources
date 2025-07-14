

- Model I/O
- MDLTransform
-  init(matrix:resetsTransform:) 

Initializer

# init(matrix:resetsTransform:)

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(
    matrix: matrix_float4x4,
    resetsTransform: Bool
)
```

## See Also

### Creating a Transform Object

convenience init(identity: ())

Initializes a transform object to the identity transformation.

Deprecated

convenience init(matrix: matrix_float4x4)

Initializes a transform object with the specified transform matrix.

convenience init(transformComponent: any MDLTransformComponent)

Initializes a transform object to match the specified transform component.

convenience init(transformComponent: any MDLTransformComponent, resetsTransform: Bool)

