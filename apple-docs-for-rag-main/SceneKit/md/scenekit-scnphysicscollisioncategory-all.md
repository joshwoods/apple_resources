

- SceneKit
- SCNPhysicsCollisionCategory
-  all 

Type Property

# all

This is the default value for a physics body’s collisionBitMask property.

iOSiPadOSMac Catalyst 13.1+macOS 10.10+tvOSvisionOSwatchOS

``` source
static var all: SCNPhysicsCollisionCategory { get }
```

## Discussion

With this collision mask, a physics body can collide with all other physics bodies.

## See Also

### Constants

static var `default`: SCNPhysicsCollisionCategory

The default categoryBitMask value for dynamic and kinematic bodies.

static var `static`: SCNPhysicsCollisionCategory

The default categoryBitMask value for static bodies.

