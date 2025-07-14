

- UIKit
- UICollisionBehavior
- UICollisionBehavior.Mode
-  everything 

Type Property

# everything

Specifies that the dynamic items, associated with the collision behavior, collide with each other *and* with specified collision boundaries.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
static var everything: UICollisionBehavior.Mode { get }
```

## Discussion

This is the default collision behavior mode.

## See Also

### Constants

static var items: UICollisionBehavior.Mode

Specifies that the dynamic items, associated with the collision behavior, collide only with each other and not with specified collision boundaries.

static var boundaries: UICollisionBehavior.Mode

Specifies that the dynamic items, associated with the collision behavior, collide only with specified collision boundaries and don’t collide with each other.

