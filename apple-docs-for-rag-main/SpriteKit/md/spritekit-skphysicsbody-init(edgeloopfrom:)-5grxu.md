

- SpriteKit
- SKPhysicsBody
-  init(edgeLoopFrom:) 

Initializer

# init(edgeLoopFrom:)

Creates an edge loop from a path.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(edgeLoopFrom path: CGPath)
```

## Parameters 

`path`  

A Core Graphics path. The points are specified relative to the owning node’s origin. The path must not intersect itself.

## Return Value

A new edge-based physics body.

## Mentioned in 

Shaping a Physics Body to Match a Node’s Graphics

## Discussion

If the path is not already closed, a loop is automatically created by joining the last point to the first.

An edge has no volume or mass and is always treated as if the isDynamic property is equal to false. Edges may only collide with volume-based physics bodies.

## See Also

### Creating an Edge-Based Physics Body

Creating an Edge Loop Around a Scene

Border your scene with an obstacle that physics bodies cannot penetrate.

init(edgeLoopFrom: CGRect)

Creates an edge loop from a rectangle.

init(edgeFrom: CGPoint, to: CGPoint)

Creates an edge between two points.

init(edgeChainFrom: CGPath)

Creates an edge chain from a path.

