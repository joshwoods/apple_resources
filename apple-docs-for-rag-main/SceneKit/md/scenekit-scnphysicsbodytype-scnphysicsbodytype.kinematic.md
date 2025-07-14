

- SceneKit
- SCNPhysicsBodyType
-  SCNPhysicsBodyType.kinematic 

Case

# SCNPhysicsBodyType.kinematic

A physics body that is unaffected by forces or collisions but that can cause collisions affecting other bodies when moved.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case kinematic
```

## Discussion

Use kinematic bodies for scene elements that you want to control directly directly but whose movement manipulates other elements. For example, to allow the user to push objects around with a finger, you might create a kinematic body and attach it to an invisible node that you move to follow touch events. (In macOS, use the same technique to allow the user to move objects with the mouse pointer.)

## See Also

### Constants

case `static`

A physics body that is unaffected by forces or collisions and cannot move.

case dynamic

A physics body that can be affected by forces and collisions.

