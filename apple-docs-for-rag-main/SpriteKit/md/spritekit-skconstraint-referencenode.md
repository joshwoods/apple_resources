

- SpriteKit
- SKConstraint
-  referenceNode 

Instance Property

# referenceNode

The node whose coordinate system should be used to apply the constraint.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOSvisionOS 1.0+watchOS 2.0+

``` source
var referenceNode: SKNode? { get set }
```

## Discussion

The default value is `nil`, meaning that the coordinate system of the node’s parent is used to apply the constraint. If another node is specified, all positions are converted into this node’s coordinate system before the constraint is applied.

