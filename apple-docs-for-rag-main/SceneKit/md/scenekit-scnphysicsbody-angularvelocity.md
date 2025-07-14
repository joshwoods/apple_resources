

- SceneKit
- SCNPhysicsBody
-  angularVelocity 

Instance Property

# angularVelocity

A vector describing both the current rotation axis and rotational speed (in radians per second) of the physics body.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var angularVelocity: SCNVector4 { get set }
```

## Discussion

A positive rotational speed indicates counterclockwise rotation (when viewed from the direction the rotation axis points in).

SceneKit’s physics simulation determines the angular velocity (and corresponding change in rotation) of each dynamic physics body in the scene. You can also set a body’s velocity directly to set the physics simulation in motion or influence its behavior.

The effect of reading or setting this property’s value changes based on the current context:

- When invoked within a rendering loop method (any of the methods in the SCNSceneRendererDelegate protocol), or from any other code invoked from within such a method, reading the property returns the current result of the physics simulation, and setting the property immediately applies the change.

- When invoked at any other time, reading the property returns the last value set for the property, and setting the property does not take effect until the next pass through the rendering loop.

## See Also

### Interacting with Bodies in Motion

var velocity: SCNVector3

A vector describing both the current speed (in meters per second) and direction of motion of the physics body.

