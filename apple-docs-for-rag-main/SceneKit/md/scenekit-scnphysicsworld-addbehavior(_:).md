

- SceneKit
- SCNPhysicsWorld
-  addBehavior(\_:) 

Instance Method

# addBehavior(\_:)

Adds a behavior to the physics world.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func addBehavior(_ behavior: SCNPhysicsBehavior)
```

## Parameters 

`behavior`  

The behavior to be added.

## Discussion

Physics behaviors constrain or modify the effects of the physics simulation on sets of physics bodies. For example, the SCNPhysicsHingeJoint behavior causes two bodies to move as if connected by a hinge that pivots around a specific axis, and the SCNPhysicsVehicle behavior causes a body to roll like a car or other wheeled vehicle.

To use a behavior in your scene, follow these steps:

1.  Create SCNPhysicsBody objects and attach them to each node that participates in the behavior.

2.  Create and configure a behavior object joining the physics bodies. See SCNPhysicsBehavior for a list of behavior classes.

3.  Call addBehavior(_:) on your scene’s physics world object to add the behavior to the physics simulation.

## See Also

### Registering Physics Behaviors

func removeBehavior(SCNPhysicsBehavior)

Removes a behavior from the physics world.

var allBehaviors: [SCNPhysicsBehavior]

The list of behaviors affecting bodies in the physics world.

func removeAllBehaviors()

Removes all behaviors affecting bodies in the physics world.

