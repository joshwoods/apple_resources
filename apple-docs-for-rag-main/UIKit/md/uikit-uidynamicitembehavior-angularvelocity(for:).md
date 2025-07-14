

- UIKit
- UIDynamicItemBehavior
-  angularVelocity(for:) 

Instance Method

# angularVelocity(for:)

Returns the angular velocity for a specified dynamic item.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func angularVelocity(for item: any UIDynamicItem) -> CGFloat
```

## Parameters 

`item`  

The dynamic item whose angular velocity you want to get.

## Return Value

The angular velocity of the specified dynamic item, in radians per second.

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

var isAnchored: Bool

A Boolean value indicating whether the item is anchored to its current position.

