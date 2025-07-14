

- RealityKit
-  BlendWeight 

Enumeration

# BlendWeight

A numerical representation of the impact an animation has on a scene or entity.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum BlendWeight
```

## Overview

The BlendTreeSourceNode structure accepts this enumeration as an initializer argument.

To specify a custom weight, use the value case:

```
let node = BlendTreeSourceNode(
    source: animation1,
    name: "anim2",
    weight: .value(0.75))
```

## Topics

### Choosing the blend weight

case bindTarget(BindTarget, defaultWeight: Float)

The amount of impact an animation has on the bind target of an entity.

case parameter(String, defaultWeight: Float)

The amount of impact an animation has on a named parameter of an entity.

case value(Float)

The numerical representation of the impact an animation has on an entity.

### Comparing blend weights

static func == (BlendWeight, BlendWeight) -> Bool

Returns a Boolean value that indicates whether two blend weights are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

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

struct BlendTreeInvalidNode

A blend tree node that’s internal only or sources from an invalid definition.

