

- SceneKit
- SCNPhysicsBodyType
-  SCNPhysicsBodyType.static 

Case

# SCNPhysicsBodyType.static

A physics body that is unaffected by forces or collisions and cannot move.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
case `static`
```

## Discussion

Use static bodies to construct fixtures in your scene that other bodies need to collide with but that do not themselves move, such as floors, walls, and terrain.

## See Also

### Constants

case dynamic

A physics body that can be affected by forces and collisions.

case kinematic

A physics body that is unaffected by forces or collisions but that can cause collisions affecting other bodies when moved.

