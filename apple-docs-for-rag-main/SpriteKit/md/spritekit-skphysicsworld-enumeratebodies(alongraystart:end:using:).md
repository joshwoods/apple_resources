

- SpriteKit
- SKPhysicsWorld
-  enumerateBodies(alongRayStart:end:using:) 

Instance Method

# enumerateBodies(alongRayStart:end:using:)

Enumerates all the physics bodies in the scene that intersect a ray.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func enumerateBodies(
    alongRayStart start: CGPoint,
    end: CGPoint,
    using block: @escaping (SKPhysicsBody, CGPoint, CGVector, UnsafeMutablePointer) -> Void
)
```

## Parameters 

`start`  

The starting point for the ray in scene coordinates.

`end`  

The ending point for the ray in scene coordinates.

`block`  

A block to be called for each physics body that the ray touches. The block takes the following parameters:

body  
The physics body that the ray intersected.

point  
The point in scene coordinates where the ray contacted the physics body.

normal  
The normal vector for the physics body at the point of contact.

stop  
A pointer to a Boolean variable. Your block can set this to true to terminate the enumeration.

## Mentioned in 

Searching the World for Physics Bodies

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

func enumerateBodies(at: CGPoint, using: (SKPhysicsBody, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that contain a point.

func enumerateBodies(in: CGRect, using: (SKPhysicsBody, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that intersect the specified rectangle.

