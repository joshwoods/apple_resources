

- GameplayKit
- GKQuadtreeNode
-  quad 

Instance Property

# quad

The axis-aligned bounding rectangle represented by the node.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
var quad: GKQuad { get }
```

## Discussion

You can use this rectangle to find elements in the tree with the elements(in:) method.

