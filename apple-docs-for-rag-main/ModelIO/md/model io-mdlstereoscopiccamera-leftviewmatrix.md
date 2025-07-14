

- Model I/O
- MDLStereoscopicCamera
-  leftViewMatrix 

Instance Property

# leftViewMatrix

The transformation matrix that determines the position and orientation of the camera’s left viewpoint relative to a scene.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var leftViewMatrix: matrix_float4x4 { get }
```

## Discussion

Model I/O automatically generates this matrix from the camera’s position and orientation, additionally using the interPupillaryDistance and leftVergence properties to account for the offset and angle of a stereoscopic camera’s left viewpoint.

A renderer uses this matrix, along with the leftProjectionMatrix property and model matrices derived from the camera’s position and orientation (the transform property) and the content to be rendered, to transform vertex data to the renderer’s 2D screen space at render time.

## See Also

### Generating View and Projection Matrices

var leftProjectionMatrix: matrix_float4x4

The transformation matrix that determines the extent of a scene visible to the camera’s left viewpoint.

var rightViewMatrix: matrix_float4x4

The transformation matrix that determines the position and orientation of the camera’s right viewpoint relative to a scene.

var rightProjectionMatrix: matrix_float4x4

The transformation matrix that determines the extent of a scene visible to the camera’s right viewpoint.

