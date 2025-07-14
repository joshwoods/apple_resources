

- SceneKit
- SCNPhysicsWorld
-  removeBehavior(\_:) 

Instance Method

# removeBehavior(\_:)

Removes a behavior from the physics world.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
func removeBehavior(_ behavior: SCNPhysicsBehavior)
```

## Parameters 

`behavior`  

The behavior to be removed.

## See Also

### Registering Physics Behaviors

func addBehavior(SCNPhysicsBehavior)

Adds a behavior to the physics world.

var allBehaviors: [SCNPhysicsBehavior]

The list of behaviors affecting bodies in the physics world.

func removeAllBehaviors()

Removes all behaviors affecting bodies in the physics world.

