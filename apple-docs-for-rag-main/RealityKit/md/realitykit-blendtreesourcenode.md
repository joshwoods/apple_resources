

- RealityKit
-  BlendTreeSourceNode 

Structure

# BlendTreeSourceNode

A blend node that contains an animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct BlendTreeSourceNode
```

## Overview

This structure adopts BlendTreeNode and adds the ability to store a single animation. A complete BlendTreeAnimation represents a mix of all the animations that its source nodes contain. Each source node defines a weight that determines how much effect the source’s animation has in the blend tree’s resulting, mixed animation. To define the source’s animation, set this structure’s source property.

### Access a source node of a blend tree

A source may exist in any leaf-node position in the blend animation’s tree. The following code checks the root node for a source. If instead the root node is a branch, the code begins checking the branches sources.

```
// Check if the root node is a source.
if let blendNode = blendTree.root as? BlendTreeSourceNode {
    // Found a source.

// Check if the root node is a branch.
} else if let source = blendTree.root as? BlendTreeBlendNode {

        // Check for a source in the branch's sources.
        if let source = blendNode.sources[0] as? BlendTreeSourceNode {
            // Found a source.
        }
    }
}
```

## Topics

### Creating a blend tree animation node

init(source: any AnimationDefinition, name: String, weight: BlendWeight)

Creates a node that defines an animation within a tree of other blend nodes.

### Configuring a blend tree animation node

var name: String

A textual name for the blend node.

var source: (any AnimationDefinition)?

The blend node’s animation.

var weight: BlendWeight

A normalized percentage that designates how much effect this node has compared to peer nodes.

## Relationships

### Conforms To

- BlendTreeNode

## See Also

### Blend trees

struct BlendTreeAnimation

A collection of animations on the same property that the framework blends to a single animation.

protocol BlendTreeNode

An interface for a node that’s a member of a blend tree.

struct BlendTreeBlendNode

A source node for an animation that mixes several animations to form a single animation.

struct BlendTreeInvalidNode

A blend tree node that’s internal only or sources from an invalid definition.

enum BlendWeight

A numerical representation of the impact an animation has on a scene or entity.

