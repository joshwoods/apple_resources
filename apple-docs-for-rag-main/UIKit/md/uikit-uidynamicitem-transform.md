

- UIKit
- UIDynamicItem
-  transform 

Instance Property

# transform

The rotation of the dynamic item.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var transform: CGAffineTransform { get set }
```

**Required**

## Discussion

UIKit Dynamics makes use only of the rotation value in this property.

The dynamic animator (that the item is associated with) calls this method when it has computed a new rotation value for the item.

## See Also

### Participating in dynamic animation

var bounds: CGRect

Called when a dynamic animator needs the bounds of the dynamic item.

**Required**

var center: CGPoint

The center point of the dynamic item.

**Required**

var collisionBoundsType: UIDynamicItemCollisionBoundsType

The type of collision bounds associated with the item.

var collisionBoundingPath: UIBezierPath

The path-based shape to use for the collision bounds.

