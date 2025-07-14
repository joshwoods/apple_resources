

- UIKit
- UICollisionBehavior
-  setTranslatesReferenceBoundsIntoBoundary(with:) 

Instance Method

# setTranslatesReferenceBoundsIntoBoundary(with:)

Specifies a collision boundary based on the bounds of the animation reference system, with optional insets.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func setTranslatesReferenceBoundsIntoBoundary(with insets: UIEdgeInsets)
```

## Parameters 

`insets`  

Insets to apply to the reference system’s bounds when defining the collision boundary.

## Discussion

The result of using this method depends on how you’ve initialized the dynamic animator (of class UIDynamicAnimator) that you’ve added the collision behavior to. See the overview in UIDynamicAnimator for a discussion of initialization options and modes for animators.

Here is how the dynamic animator’s initialization impacts use of this method:

- For a view-only dynamic animator, the reference bounds are those of the reference view

- For a collection-view dynamic animator, the reference bounds are those of the collection view layout

- For a dynamic-item dynamic animator, there are no reference bounds.

For a collision behavior added to a view-only or collection-view dynamic animator, activate a reference-system-based collision boundary by setting the translatesReferenceBoundsIntoBoundary property to true.

## See Also

### Configuring a collision behavior

func addBoundary(withIdentifier: any NSCopying, for: UIBezierPath)

Adds a collision boundary, specified as a Bezier path, to the collision behavior.

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

var translatesReferenceBoundsIntoBoundary: Bool

Specifies whether a boundary based on the reference system is active.

