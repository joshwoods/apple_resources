

- UIKit
- UIDynamicItem
-  collisionBoundingPath 

Instance Property

# collisionBoundingPath

The path-based shape to use for the collision bounds.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional var collisionBoundingPath: UIBezierPath { get }
```

## Discussion

When the collisionBoundsType property is UIDynamicItemCollisionBoundsType.path, the object in this property is used as the collision bounds. If your dynamic item implements the collisionBoundsType property, you must also implement this property.

The path object you create must represent a convex polygon with counter-clockwise or clockwise winding, and the path must not intersect itself. The (0, 0) point of the path must be located at the center point of the corresponding dynamic item. If the center point does not match the path’s origin, collision behaviors may not work as expected.

## See Also

### Participating in dynamic animation

var bounds: CGRect

Called when a dynamic animator needs the bounds of the dynamic item.

**Required**

var center: CGPoint

The center point of the dynamic item.

**Required**

var transform: CGAffineTransform

The rotation of the dynamic item.

**Required**

var collisionBoundsType: UIDynamicItemCollisionBoundsType

The type of collision bounds associated with the item.

