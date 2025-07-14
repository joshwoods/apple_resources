

- SpriteKit
- SKPhysicsWorld
-  body(in:) 

Instance Method

# body(in:)

Searches for the first physics body that intersects the specified rectangle.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func body(in rect: CGRect) -> SKPhysicsBody?
```

## Parameters 

`rect`  

A rectangle in scene coordinates.

## Return Value

The first physics body discovered that intersects the rectangle. If no body intersects the rectangle, this method returns `nil`.

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

func enumerateBodies(alongRayStart: CGPoint, end: CGPoint, using: (SKPhysicsBody, CGPoint, CGVector, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that intersect a ray.

func enumerateBodies(at: CGPoint, using: (SKPhysicsBody, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that contain a point.

func enumerateBodies(in: CGRect, using: (SKPhysicsBody, UnsafeMutablePointer&lt;ObjCBool>) -> Void)

Enumerates all the physics bodies in the scene that intersect the specified rectangle.

