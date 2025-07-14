

- SpriteKit
- SKConstraint
-  distance(\_:to:) 

Type Method

# distance(\_:to:)

Creates a constraint that keeps a node within a certain distance of a point.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
class func distance(
    _ range: SKRange,
    to point: CGPoint
) -> Self
```

## Parameters 

`range`  

The range of allowed distances between the node and the point.

`point`  

A point in the coordinate system of the node’s parent that is used to calculate the distance.

## Return Value

A new constraint.

## Discussion

Each time when constraints are applied, a line is projected between the node’s position and the target point. The distance between the two points is calculated, and if it lies outside the specified range, the node is pushed or pulled along this line until it lies within the range.

## See Also

### Creating Distance Constraints

class func distance(SKRange, to: SKNode) -> Self

Creates a constraint that keeps a node within a certain distance of another node.

class func distance(SKRange, to: CGPoint, in: SKNode) -> Self

Creates a constraint that keeps a node within a certain distance of a point in another node’s coordinate system.

