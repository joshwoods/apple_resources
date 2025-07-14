

- RealityKit
- BlendTreeNode
-  weight 

Instance Property

# weight

A normalized percentage that designates how much effect this node has relative to peer nodes.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var weight: BlendWeight { get set }
```

**Required**

## Discussion

The value of this property relates to the node’s peers in a sources array. The sum of all node weights in a given sources array needs to equal `1.0`.

## See Also

### Configuring the blend tree node

var name: String

A textual name for the blend node.

**Required**

