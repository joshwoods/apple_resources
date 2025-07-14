

- RealityKit
- BlendTreeBlendNode
-  sources 

Instance Property

# sources

The nodes that branch from a node to form part of a blend tree.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
var sources: [any BlendTreeNode]
```

## Discussion

This node combines the animations of each member of this array to a single animation that represents a *blend* of the sources. If a source is a BlendTreeSourceNode, this structure blends its animation into the output. If a source is a BlendTreeBlendNode, this structure blends the output of its sources into this structure’s output.

