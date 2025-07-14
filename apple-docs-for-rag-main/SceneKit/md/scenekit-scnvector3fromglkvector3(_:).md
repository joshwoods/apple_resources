

- SceneKit
-  SCNVector3FromGLKVector3(\_:) 

Function

# SCNVector3FromGLKVector3(\_:)

Returns a three-element SceneKit vector structure corresponding to a GLKit vector structure.

iOSiPadOSmacOStvOS

``` source
func SCNVector3FromGLKVector3(_ vector: GLKVector3) -> SCNVector3
```

## Parameters 

`vector`  

A three-element GLKit vector structure.

## Return Value

A three-element SceneKit vector structure representing the same vector as the input parameter.

## See Also

### Converting Vector Types

func SCNVector3ToGLKVector3(SCNVector3) -> GLKVector3

Returns a three-element GLKit vector structure corresponding to a SceneKit vector structure.

