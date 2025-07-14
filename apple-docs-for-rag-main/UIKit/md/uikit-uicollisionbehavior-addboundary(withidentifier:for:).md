

- UIKit
- UICollisionBehavior
-  addBoundary(withIdentifier:for:) 

Instance Method

# addBoundary(withIdentifier:for:)

Adds a collision boundary, specified as a Bezier path, to the collision behavior.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func addBoundary(
    withIdentifier identifier: any NSCopying,
    for bezierPath: UIBezierPath
)
```

## Parameters 

`identifier`  

An arbitrary identifier for the boundary you are adding.

`bezierPath`  

An arbitrary Bezier path that specifies the collision boundary you are adding.

The coordinate system and origin point for the path depend on how you’ve initialized the dynamic animator (that you’re adding the behavior to). See the overview in UIDynamicAnimator for more information.

## See Also

### Configuring a collision behavior

func addBoundary(withIdentifier: any NSCopying, from: CGPoint, to: CGPoint)

Adds a collision boundary, specified as a line segment, to the collision behavior.

var boundaryIdentifiers: [any NSCopying]?

The set of boundary identifiers that you’ve added to the collision behavior.

func boundary(withIdentifier: any NSCopying) -> UIBezierPath?

Returns a specified Bezier-path boundary.

var collisionMode: UICollisionBehavior.Mode

The type of edges that participate in collisions for the collision behavior.

func removeAllBoundaries()

Removes all previously-specified collision boundaries from the collision behavior.

func removeBoundary(withIdentifier: any NSCopying)

Removes a specific collision boundary from the collision behavior.

func setTranslatesReferenceBoundsIntoBoundary(with: UIEdgeInsets)

Specifies a collision boundary based on the bounds of the animation reference system, with optional insets.

var translatesReferenceBoundsIntoBoundary: Bool

Specifies whether a boundary based on the reference system is active.

