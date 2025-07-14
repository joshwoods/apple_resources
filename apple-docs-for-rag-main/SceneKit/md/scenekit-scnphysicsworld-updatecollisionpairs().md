

- SceneKit
- SCNPhysicsWorld
-  updateCollisionPairs() 

Instance Method

# updateCollisionPairs()

Forces the physics engine to reevaluate possible collisions between physics bodies.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func updateCollisionPairs()
```

## Discussion

By default, SceneKit checks for collisions between physics bodies only once per simulation step. If you directly change the positions of any physics bodies outside of a SCNPhysicsContactDelegate method, call the updateCollisionPairs() method before using any of the methods listed in Searching for Physics Bodies Detecting Contacts Between Physics Bodies.

## See Also

### Related Documentation

var contactDelegate: (any SCNPhysicsContactDelegate)?

A delegate that is called when two physics bodies come in contact with each other.

### Managing the Physics Simulation

var gravity: SCNVector3

A vector that specifies the gravitational acceleration applied to physics bodies in the physics world.

var speed: CGFloat

The rate at which the simulation executes.

var timeStep: TimeInterval

The time interval between updates to the physics simulation.

