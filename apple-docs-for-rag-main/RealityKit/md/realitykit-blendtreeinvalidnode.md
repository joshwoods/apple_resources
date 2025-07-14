

- RealityKit
-  BlendTreeInvalidNode 

Structure

# BlendTreeInvalidNode

A blend tree node that’s internal only or sources from an invalid definition.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct BlendTreeInvalidNode
```

## Overview

This structure adopts BlendTreeNode and adds the ability to detect a node that contains neither an animation nor any branches in the blend tree.

You don’t create instances of this structure. Instead, detect whether your blend-tree node matches the framework’s criteria for invalid nodes by checking the node type, as the following code demonstrates.

```
// Get the blend tree's root node.
guard let blendNode = blendTree.root as? BlendTreeBlendNode else { return }
for node in blendNode.sources {
    if let invalidNode = node as? BlendTreeInvalidNode {
        // Respond to invalid-node criteria.
```

## Topics

### Configuring the blend tree invalid node

var name: String

A textual name for the blend node.

var weight: BlendWeight

The amount that an animation impacts the entity it applies to.

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

struct BlendTreeSourceNode

A blend node that contains an animation.

enum BlendWeight

A numerical representation of the impact an animation has on a scene or entity.

