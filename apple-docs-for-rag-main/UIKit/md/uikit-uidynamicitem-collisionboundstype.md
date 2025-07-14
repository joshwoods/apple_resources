

- UIKit
- UIDynamicItem
-  collisionBoundsType 

Instance Property

# collisionBoundsType

The type of collision bounds associated with the item.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
optional var collisionBoundsType: UIDynamicItemCollisionBoundsType { get }
```

## Discussion

The dynamics system uses this property to determine how to evaluate collisions with the dynamic item. Rectangular and elliptical bounds are defined by the bounds property of the item. For custom collision bounds, the shape of the bounds are in the collisionBoundingPath property.

If you implement this property in your dynamic item and set its value to UIDynamicItemCollisionBoundsType.path, you must also implement the collisionBoundingPath property and provide a valid path. Failure to do so is a programmer error.

The default value of this property is UIDynamicItemCollisionBoundsType.rectangle.

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

var collisionBoundingPath: UIBezierPath

The path-based shape to use for the collision bounds.

