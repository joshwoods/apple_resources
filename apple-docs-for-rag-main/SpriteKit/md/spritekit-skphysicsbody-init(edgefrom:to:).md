

- SpriteKit
- SKPhysicsBody
-  init(edgeFrom:to:) 

Initializer

# init(edgeFrom:to:)

Creates an edge between two points.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
init(
    edgeFrom p1: CGPoint,
    to p2: CGPoint
)
```

## Parameters 

`p1`  

The starting point for the edge, relative to the owning node’s origin.

`p2`  

The ending point for the edge, relative to the owning node’s origin.

## Return Value

A new edge-based physics body.

## Mentioned in 

Shaping a Physics Body to Match a Node’s Graphics

## Discussion

An edge has no volume or mass and is always treated as if the isDynamic property is equal to false. Edges may only collide with volume-based physics bodies.

## See Also

### Creating an Edge-Based Physics Body

Creating an Edge Loop Around a Scene

Border your scene with an obstacle that physics bodies cannot penetrate.

init(edgeLoopFrom: CGRect)

Creates an edge loop from a rectangle.

init(edgeLoopFrom: CGPath)

Creates an edge loop from a path.

init(edgeChainFrom: CGPath)

Creates an edge chain from a path.

