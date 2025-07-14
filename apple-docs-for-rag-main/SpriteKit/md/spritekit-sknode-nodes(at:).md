

- SpriteKit
- SKNode
-  nodes(at:) 

Instance Method

# nodes(at:)

Returns an array of all visible descendants that intersect a point.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

**iOS, iPadOS, Mac Catalyst, macOS, tvOS, visionOS**

``` source
@MainActor
func nodes(at p: CGPoint) -> [SKNode]
```

**watchOS**

``` source
func nodes(at p: CGPoint) -> [SKNode]
```

## Parameters 

`p`  

A point in the node’s coordinate system.

## Return Value

An array of all `SKNode` objects in the subtree that intersect the point. Only nodes that have an isHidden of `false` and an alpha greater that zero are included in the returned array. If no nodes intersect the point, an empty array is returned.

## Mentioned in 

Controlling User Interaction on Nodes

Understanding Hit-Testing

## Discussion

A point is considered to be in a node if it lies inside the rectangle returned by the calculateAccumulatedFrame() method.

## See Also

### Hit Testing

Understanding Hit-Testing

Learn how find child nodes at a given point by using hit-testing.

func contains(CGPoint) -> Bool

Returns a Boolean value that indicates whether a point lies inside the parent’s coordinate system.

func atPoint(CGPoint) -> SKNode

Returns the deepest visible descendant that intersects a point.

