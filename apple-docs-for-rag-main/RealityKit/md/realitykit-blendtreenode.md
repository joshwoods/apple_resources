

- RealityKit
-  BlendTreeNode 

Protocol

# BlendTreeNode

An interface for a node that’s a member of a blend tree.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
protocol BlendTreeNode
```

## Overview

This protocol specifies the common functionality for the animations that compose a BlendTreeAnimation. The animation defines a root node of this type. To define the tree, you assign the root node one of the follow structures that adopt this protocol:

- BlendTreeBlendNode, which branches the tree for every element in sources.

- BlendTreeSourceNode, which defines an animation to blend with its source property.

Note

A node in the tree may be of type BlendTreeInvalidNode, which neither specifies a list of sources nor an animation.

Each node type supplies a name and weight, which you can set during or after initialization.

```
let animation1 = FromToByAnimation(...)

let blendNode = BlendTreeSourceNode(
    source: animation1,
    name: "Anim1",
    weight: .value(0.25))
```

## Topics

### Configuring the blend tree node

var name: String

A textual name for the blend node.

**Required**

var weight: BlendWeight

A normalized percentage that designates how much effect this node has relative to peer nodes.

**Required**

### Blending animations

func blend(sources: [any BlendTreeNode], name: String, isAdditive: Bool) -> any BlendTreeNode

Combines the animations that result from the individual blend-tree nodes of the given array to a single blend-tree node.

func blend(any BlendTreeNode, any BlendTreeNode, name: String, isAdditive: Bool) -> any BlendTreeNode

Combines the animations that result from two blend-tree nodes into a single blend-tree node.

## Relationships

### Conforming Types

- BlendTreeBlendNode
- BlendTreeInvalidNode
- BlendTreeSourceNode

## See Also

### Blend trees

struct BlendTreeAnimation

A collection of animations on the same property that the framework blends to a single animation.

struct BlendTreeBlendNode

A source node for an animation that mixes several animations to form a single animation.

struct BlendTreeSourceNode

A blend node that contains an animation.

struct BlendTreeInvalidNode

A blend tree node that’s internal only or sources from an invalid definition.

enum BlendWeight

A numerical representation of the impact an animation has on a scene or entity.

