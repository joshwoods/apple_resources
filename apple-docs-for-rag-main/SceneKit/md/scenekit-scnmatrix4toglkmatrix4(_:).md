

- SceneKit
-  SCNMatrix4ToGLKMatrix4(\_:) 

Function

# SCNMatrix4ToGLKMatrix4(\_:)

Returns a GLKit matrix corresponding to a SceneKit matrix.

iOSiPadOSmacOS 10.10+tvOS

**iOS, iPadOS, tvOS**

``` source
func SCNMatrix4ToGLKMatrix4(_ mat: SCNMatrix4) -> GLKMatrix4
```

**macOS**

``` source
func SCNMatrix4ToGLKMatrix4(_ mat: SCNMatrix4) -> GLKMatrix4
```

## Parameters 

`mat`  

A SceneKit matrix.

## Return Value

A GLKit matrix representing the same 3D transformation.

## See Also

### Converting Matrix Types

func SCNMatrix4FromGLKMatrix4(GLKMatrix4) -> SCNMatrix4

Returns a SceneKit matrix corresponding to a GLKit matrix.

