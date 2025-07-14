

- RealityKit
-  BlendTreeBlendNode 

Structure

# BlendTreeBlendNode

A source node for an animation that mixes several animations to form a single animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct BlendTreeBlendNode
```

## Overview

A *blend tree animation* mixes multiple animations to form a single animation. The BlendTreeBlendNode structure adopts the BlendTreeNode protocol, which specifies the behavior of animations that make up a blend tree animation. This structure adds the ability to branch a blend tree at any point. Each member of this property’s sources array represents a branch in the tree. For more information about blend trees, see BlendTreeAnimation.

## Topics

### Creating a blend-tree blend node

init(sources: [any BlendTreeNode], name: String, weight: BlendWeight, isAdditive: Bool)

Creates a tree node made up of multiple branches.

### Configuring the node

var name: String

A textual name for the blend node.

var weight: BlendWeight

A normalized percentage that designates how much effect this node has compared to peer nodes.

var isAdditive: Bool

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

### Configuring child nodes

var sources: [any BlendTreeNode]

The nodes that branch from a node to form part of a blend tree.

## Relationships

### Conforms To

- BlendTreeNode

## See Also

### Blend trees

struct BlendTreeAnimation

A collection of animations on the same property that the framework blends to a single animation.

protocol BlendTreeNode

An interface for a node that’s a member of a blend tree.

struct BlendTreeSourceNode

A blend node that contains an animation.

struct BlendTreeInvalidNode

A blend tree node that’s internal only or sources from an invalid definition.

enum BlendWeight

A numerical representation of the impact an animation has on a scene or entity.

