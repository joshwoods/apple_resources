

- SpriteKit
- SKPhysicsWorld
-  body(at:) 

Instance Method

# body(at:)

Searches for the first physics body that contains a point.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func body(at point: CGPoint) -> SKPhysicsBody?
```

## Parameters 

`point`  

A point in scene coordinates.

## Return Value

The first physics body discovered that contains the point. If no body contains the point, this method returns `nil`.

## Mentioned in 

Searching the World for Physics Bodies

## See Also

### Searching the Scene for Physics Bodies

Searching the World for Physics Bodies

Cast a ray to find the physics bodies in the scene that intersect it.

func body(alongRayStart: CGPoint, end: CGPoint) -> SKPhysicsBody?

Searches for the first physics body that intersects a ray.

func body(in: CGRect) -> SKPhysicsBody?

Searches for the first physics body that intersects the specified rectangle.

func enumerateBodies(alongRayStart: CGPoint, end: CGPoint, using: (SKPhysicsBody, CGPoint, CGVector, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that intersect a ray.

func enumerateBodies(at: CGPoint, using: (SKPhysicsBody, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that contain a point.

func enumerateBodies(in: CGRect, using: (SKPhysicsBody, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that intersect the specified rectangle.

