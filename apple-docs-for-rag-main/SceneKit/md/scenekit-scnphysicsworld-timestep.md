

- SceneKit
- SCNPhysicsWorld
-  timeStep 

Instance Property

# timeStep

The time interval between updates to the physics simulation.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var timeStep: TimeInterval { get set }
```

## Discussion

SceneKit processes the physics simulation and updates the state of all physics bodies once per the time interval specified by this property. The default value is 1/60 second (a rate of 60 Hz).

A faster simulation rate provides more accuracy in simulation results—such as collisions between fast-moving objects—but at a higher cost in CPU time (which may in turn slow down your app’s rendering frame rate). Typically, you should set this property to match your target rendering frame rate (as defined by the preferredFramesPerSecond property of the SCNView object rendering your scene).

## See Also

### Managing the Physics Simulation

var gravity: SCNVector3

A vector that specifies the gravitational acceleration applied to physics bodies in the physics world.

var speed: CGFloat

The rate at which the simulation executes.

func updateCollisionPairs()

Forces the physics engine to reevaluate possible collisions between physics bodies.

