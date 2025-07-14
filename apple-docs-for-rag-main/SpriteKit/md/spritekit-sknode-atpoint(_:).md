

- SpriteKit
- SKNode
-  atPoint(\_:) 

Instance Method

# atPoint(\_:)

Returns the deepest visible descendant that intersects a point.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**watchOS**

``` source
func atPoint(_ p: CGPoint) -> SKNode
```

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func atPoint(_ p: CGPoint) -> SKNode
```

## Parameters 

`p`  

A point in the node’s coordinate system.

## Return Value

A descendant in the subtree that intersects the point, or the receiver if no nodes intersect the point. Only nodes that have an isHidden of `false` and an alpha greater that zero are returned. If multiple descendants intersect the point, the deepest node in the tree is returned. If multiple nodes are at the same level, the intersecting node with the largest z position is returned.

## Mentioned in 

Understanding Hit-Testing

Controlling User Interaction on Nodes

## Discussion

A point is considered to be in a node if it lies inside the rectangle returned by the calculateAccumulatedFrame() method.

## See Also

### Hit Testing

Understanding Hit-Testing

Learn how find child nodes at a given point by using hit-testing.

func contains(CGPoint) -> Bool

Returns a Boolean value that indicates whether a point lies inside the parent’s coordinate system.

func nodes(at: CGPoint) -> [SKNode]

Returns an array of all visible descendants that intersect a point.

