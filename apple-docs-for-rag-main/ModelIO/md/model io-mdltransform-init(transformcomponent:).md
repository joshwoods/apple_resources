

- Model I/O
- MDLTransform
-  init(transformComponent:) 

Initializer

# init(transformComponent:)

Initializes a transform object to match the specified transform component.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
convenience init(transformComponent component: any MDLTransformComponent)
```

## Parameters 

`component`  

The component whose transform information is to be copied.

## Return Value

A new transform object.

## Discussion

Use this method to copy transformation from any object that adopts the MDLTransformComponent protocol (such as another MDLTransform instance).

## See Also

### Creating a Transform Object

convenience init(identity: ())

Initializes a transform object to the identity transformation.

Deprecated

convenience init(matrix: matrix_float4x4)

Initializes a transform object with the specified transform matrix.

convenience init(matrix: matrix_float4x4, resetsTransform: Bool)

convenience init(transformComponent: any MDLTransformComponent, resetsTransform: Bool)

