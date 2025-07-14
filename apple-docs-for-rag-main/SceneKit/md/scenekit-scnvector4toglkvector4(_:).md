

- SceneKit
-  SCNVector4ToGLKVector4(\_:) 

Function

# SCNVector4ToGLKVector4(\_:)

Returns a four-element GLKit vector structure corresponding to a SceneKit vector structure.

iOSiPadOSmacOStvOS

``` source
func SCNVector4ToGLKVector4(_ vector: SCNVector4) -> GLKVector4
```

## Parameters 

`vector`  

A four-element SceneKit vector structure.

## Return Value

A four-element GLKit vector structure representing the same vector as the input parameter.

## See Also

### Converting Vector Types

func SCNVector4FromGLKVector4(GLKVector4) -> SCNVector4

Returns a four-element SceneKit vector structure corresponding to a GLKit vector structure.

