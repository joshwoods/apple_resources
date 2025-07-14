

- SceneKit
-  SCNVector4FromGLKVector4(\_:) 

Function

# SCNVector4FromGLKVector4(\_:)

Returns a four-element SceneKit vector structure corresponding to a GLKit vector structure.

iOSiPadOSmacOStvOS

``` source
func SCNVector4FromGLKVector4(_ vector: GLKVector4) -> SCNVector4
```

## Parameters 

`vector`  

A four-element GLKit vector structure.

## Return Value

A four-element SceneKit vector structure representing the same vector as the input parameter.

## See Also

### Converting Vector Types

func SCNVector4ToGLKVector4(SCNVector4) -> GLKVector4

Returns a four-element GLKit vector structure corresponding to a SceneKit vector structure.

