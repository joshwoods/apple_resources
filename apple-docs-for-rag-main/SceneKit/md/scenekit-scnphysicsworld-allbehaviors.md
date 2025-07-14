

- SceneKit
- SCNPhysicsWorld
-  allBehaviors 

Instance Property

# allBehaviors

The list of behaviors affecting bodies in the physics world.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
var allBehaviors: [SCNPhysicsBehavior] { get }
```

## See Also

### Registering Physics Behaviors

func addBehavior(SCNPhysicsBehavior)

Adds a behavior to the physics world.

func removeBehavior(SCNPhysicsBehavior)

Removes a behavior from the physics world.

func removeAllBehaviors()

Removes all behaviors affecting bodies in the physics world.

