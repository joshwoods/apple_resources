

- SpriteKit
- SKConstraint
-  distance(\_:to:in:) 

Type Method

# distance(\_:to:in:)

Creates a constraint that keeps a node within a certain distance of a point in another node’s coordinate system.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func distance(
    _ range: SKRange,
    to point: CGPoint,
    in node: SKNode
) -> Self
```

## Parameters 

`range`  

The range of allowed distances.

`point`  

The point to use as the target point.

`node`  

The node whose coordinate system the point is specified in.

## Return Value

A new constraint.

## Discussion

Each time when constraints are applied, a line is projected between the node’s position and the target point. The distance between the two points is calculated, and if it lies outside the specified range, the node is pushed or pulled along this line until it lies within the range.

## See Also

### Creating Distance Constraints

class func distance(SKRange, to: SKNode) -> Self

Creates a constraint that keeps a node within a certain distance of another node.

class func distance(SKRange, to: CGPoint) -> Self

Creates a constraint that keeps a node within a certain distance of a point.

