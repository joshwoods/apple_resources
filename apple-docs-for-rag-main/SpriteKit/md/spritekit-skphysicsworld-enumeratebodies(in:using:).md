

- SpriteKit
- SKPhysicsWorld
-  enumerateBodies(in:using:) 

Instance Method

# enumerateBodies(in:using:)

Enumerates all the physics bodies in the scene that intersect the specified rectangle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func enumerateBodies(
    in rect: CGRect,
    using block: @escaping (SKPhysicsBody, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`rect`  

A rectangle in scene coordinates.

`block`  

A block to be called for each physics body that contains the point. The block takes the following parameters:

body  
The physics body that intersected the rectangle.

stop  
A pointer to a Boolean variable. Your block can set this to true to terminate the enumeration.

## See Also

### Searching the Scene for Physics Bodies

Searching the World for Physics Bodies

Cast a ray to find the physics bodies in the scene that intersect it.

func body(alongRayStart: CGPoint, end: CGPoint) -> SKPhysicsBody?

Searches for the first physics body that intersects a ray.

func body(at: CGPoint) -> SKPhysicsBody?

Searches for the first physics body that contains a point.

func body(in: CGRect) -> SKPhysicsBody?

Searches for the first physics body that intersects the specified rectangle.

func enumerateBodies(alongRayStart: CGPoint, end: CGPoint, using: (SKPhysicsBody, CGPoint, CGVector, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that intersect a ray.

func enumerateBodies(at: CGPoint, using: (SKPhysicsBody, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that contain a point.

