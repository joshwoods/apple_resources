

- UIKit
- UIDynamicItemBehavior
-  isAnchored 

Instance Property

# isAnchored

A Boolean value indicating whether the item is anchored to its current position.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var isAnchored: Bool { get set }
```

## Discussion

An anchored item participates in collisions but is not affected by those collisions. Instead, the item behaves like a collision boundary. The default value of this property is false.

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

var friction: CGFloat

The linear resistance for the behavior’s dynamic items when two slide against each other.

var resistance: CGFloat

The linear resistance for the behavior’s dynamic items, which reduces their linear velocity over time.

var charge: CGFloat

The charge associated with the item.

