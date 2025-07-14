

- SceneKit
-  SCNMatrix4FromGLKMatrix4(\_:) 

Function

# SCNMatrix4FromGLKMatrix4(\_:)

Returns a SceneKit matrix corresponding to a GLKit matrix.

iOSiPadOSmacOS 10.10+tvOS

**iOS, iPadOS, tvOS**

``` source
func SCNMatrix4FromGLKMatrix4(_ mat: GLKMatrix4) -> SCNMatrix4
```

**macOS**

``` source
func SCNMatrix4FromGLKMatrix4(_ mat: GLKMatrix4) -> SCNMatrix4
```

## Parameters 

`mat`  

A GLKit matrix.

## Return Value

A SceneKit matrix representing the same 3D transformation.

## See Also

### Converting Matrix Types

func SCNMatrix4ToGLKMatrix4(SCNMatrix4) -> GLKMatrix4

Returns a GLKit matrix corresponding to a SceneKit matrix.

