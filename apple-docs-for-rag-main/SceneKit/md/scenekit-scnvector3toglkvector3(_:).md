

- SceneKit
-  SCNVector3ToGLKVector3(\_:) 

Function

# SCNVector3ToGLKVector3(\_:)

Returns a three-element GLKit vector structure corresponding to a SceneKit vector structure.

iOSiPadOSmacOStvOS

``` source
func SCNVector3ToGLKVector3(_ vector: SCNVector3) -> GLKVector3
```

## Parameters 

`vector`  

A three-element SceneKit vector structure.

## Return Value

A three-element GLKit vector structure representing the same vector as the input parameter.

## See Also

### Converting Vector Types

func SCNVector3FromGLKVector3(GLKVector3) -> SCNVector3

Returns a three-element SceneKit vector structure corresponding to a GLKit vector structure.

