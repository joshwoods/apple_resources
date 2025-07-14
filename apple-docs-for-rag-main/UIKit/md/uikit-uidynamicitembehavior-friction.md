

- UIKit
- UIDynamicItemBehavior
-  friction 

Instance Property

# friction

The linear resistance for the behavior’s dynamic items when two slide against each other.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var friction: CGFloat { get set }
```

## Discussion

Default value is `0.0`, which corresponds to no friction. Use a value of `1.0` to apply strong friction. To apply an even stronger friction, you can use higher numbers.

## See Also

### Configuring a dynamic item behavior

func addAngularVelocity(CGFloat, for: any UIDynamicItem)

Adds a specified angular velocity to a dynamic item.

func addLinearVelocity(CGPoint, for: any UIDynamicItem)

Adds a specified linear velocity to a dynamic item.

var allowsRotation: Bool

Specifies whether rotation is allowed for the behavior’s dynamic items.

var angularResistance: CGFloat

The angular resistance for the behavior’s dynamic items.

func angularVelocity(for: any UIDynamicItem) -> CGFloat

Returns the angular velocity for a specified dynamic item.

func linearVelocity(for: any UIDynamicItem) -> CGPoint

Returns the linear velocity for a specified dynamic item.

var density: CGFloat

The relative mass density of the behavior’s dynamic items.

var elasticity: CGFloat

The amount of elasticity applied to collisions for the behavior’s dynamic items.

var resistance: CGFloat

The linear resistance for the behavior’s dynamic items, which reduces their linear velocity over time.

var charge: CGFloat

The charge associated with the item.

var isAnchored: Bool

A Boolean value indicating whether the item is anchored to its current position.

