

- UIKit
- UIDynamicItem
-  bounds 

Instance Property

# bounds

Called when a dynamic animator needs the bounds of the dynamic item.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var bounds: CGRect { get }
```

**Required**

## See Also

### Participating in dynamic animation

var center: CGPoint

The center point of the dynamic item.

**Required**

var transform: CGAffineTransform

The rotation of the dynamic item.

**Required**

var collisionBoundsType: UIDynamicItemCollisionBoundsType

The type of collision bounds associated with the item.

var collisionBoundingPath: UIBezierPath

The path-based shape to use for the collision bounds.

