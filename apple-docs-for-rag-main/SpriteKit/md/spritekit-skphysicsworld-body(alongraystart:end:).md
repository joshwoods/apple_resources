

- SpriteKit
- SKPhysicsWorld
-  body(alongRayStart:end:) 

Instance Method

# body(alongRayStart:end:)

Searches for the first physics body that intersects a ray.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func body(
    alongRayStart start: CGPoint,
    end: CGPoint
) -> SKPhysicsBody?
```

## Parameters 

`start`  

The starting point for the ray in scene coordinates.

`end`  

The ending point for the ray in scene coordinates.

## Return Value

The first physics body discovered that intersects the ray. This may be any body along the ray; it is not guaranteed to be the closest physics body. If no body intersects the ray, this method returns `nil`.

## See Also

### Searching the Scene for Physics Bodies

Searching the World for Physics Bodies

Cast a ray to find the physics bodies in the scene that intersect it.

func body(at: CGPoint) -> SKPhysicsBody?

Searches for the first physics body that contains a point.

func body(in: CGRect) -> SKPhysicsBody?

Searches for the first physics body that intersects the specified rectangle.

func enumerateBodies(alongRayStart: CGPoint, end: CGPoint, using: (SKPhysicsBody, CGPoint, CGVector, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that intersect a ray.

func enumerateBodies(at: CGPoint, using: (SKPhysicsBody, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that contain a point.

func enumerateBodies(in: CGRect, using: (SKPhysicsBody, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that intersect the specified rectangle.

