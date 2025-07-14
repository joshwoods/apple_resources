

- UIKit
- UIDynamicItemBehavior
-  density 

Instance Property

# density

The relative mass density of the behavior’s dynamic items.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var density: CGFloat { get set }
```

## Discussion

A dynamic item’s relative density, along with its size, determines its effective mass when it participates in UIKit Dynamics behaviors—including friction, collisions, pushes, and so on. For example, say you have two dynamic items with the same density but different sizes: item one is `100 x 100` points and item two is `100 x 200` points. In this example, item two has twice the effective mass of item one. In an elastic collision, these items exhibit a natural conservation of momentum according to their relative masses.

A `100 x 100` point dynamic item with a density of `1.0`, to which you apply a force (via a push behavior) of magnitude `1.0`, accelerates at `100` points per second².

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

var elasticity: CGFloat

The amount of elasticity applied to collisions for the behavior’s dynamic items.

var friction: CGFloat

The linear resistance for the behavior’s dynamic items when two slide against each other.

var resistance: CGFloat

The linear resistance for the behavior’s dynamic items, which reduces their linear velocity over time.

var charge: CGFloat

The charge associated with the item.

var isAnchored: Bool

A Boolean value indicating whether the item is anchored to its current position.

