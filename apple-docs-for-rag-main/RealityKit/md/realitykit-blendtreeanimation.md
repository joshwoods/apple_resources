

- RealityKit
-  BlendTreeAnimation 

Structure

# BlendTreeAnimation

A collection of animations on the same property that the framework blends to a single animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
struct BlendTreeAnimation where Value : AnimatableData
```

## Overview

This structure provides a way to form a single animation by mixing several other animations together. You define a source node for each animation, and a weight, which determines how much each individual animation takes effect in the resulting animation.

To create the blended animation, you define a *blend tree* that sprouts from root, which consists of one or more blend-tree nodes (BlendTreeNode). Each node may be one of the following conforming types:

- BlendTreeBlendNode, which branches the tree for every element in sources

- BlendTreeSourceNode, which defines one of the animations to blend via its source property

Because source nodes reference no other nodes, they represent leaf nodes in the tree.

### Blending two skeletal movements to a single movement

The following animation plays a sampling of the animations named `anim1` and `anim2`. To fine-tune the interplay between the two animations, the code sets a blend weight for each animation. The weight of `0.25` for `anim1` determines that the first animation’s behavior is 25% prominent in the final result. The `anim2` weight is `0.75`, as the cumulative blend weight across all animations in the tree needs to equal `1`. This determines that the second animation influences 75% of the visual behavior of the blended animation.

```
let anim1 = FromToByAnimation(
    name: "anim1",
    from: JointTransforms([Transform(scale: SIMD3(1, 2, 3),
    rotation: simd_quatf(ix: 5, iy: 6, iz: 7, r: 8),
    translation: SIMD3(10, 20, 30))]),
    to: JointTransforms([Transform(scale: SIMD3(11, 21, 31),
    rotation: simd_quatf(ix: 50, iy: 60, iz: 70, r: 80),
    translation: SIMD3(100, 200, 300))]),
    duration: 1.0)

let anim2 = FromToByAnimation(
    name: "anim2",
    from: JointTransforms([Transform(scale: SIMD3(10, 20, 30),
    rotation: simd_quatf(ix: 4, iy: 5, iz: 5, r: 7),
    translation: SIMD3(100, 200, 300))]),
    to: JointTransforms([Transform(scale: SIMD3(110, 210, 310),
    rotation: simd_quatf(ix: 500, iy: 60, iz: 70, r: 80),
    translation: SIMD3(1000, 2000, 3000))]),
    duration: 10.0)

let blendTree = BlendTreeAnimation(
    blend(
        BlendTreeSourceNode(
            source: anim1,
            name: "anim1",
            weight: .value(0.25)),
        BlendTreeSourceNode(
            source: anim2,
            name: "anim2",
            weight: .value(0.75)),
        name: "blend"),
    name: "blendTree",
    bindTarget: .parameter("bar")
)
```

Tip

To modify the weights for each frame, create a source node with a dynamic BlendWeight, such as with the BlendWeight.bindTarget(_:defaultWeight:) or BlendWeight.parameter(_:defaultWeight:) enumeration cases.

## Topics

### Creating an animation

init(any BlendTreeNode, name: String, isAdditive: Bool, bindTarget: BindTarget?, blendLayer: Int32, repeatMode: AnimationRepeatMode, fillMode: AnimationFillMode, trimStart: TimeInterval?, trimEnd: TimeInterval?, trimDuration: TimeInterval?, offset: TimeInterval, delay: TimeInterval, speed: Float)

Creates a unique animation from a combination of other animations in the form of a tree.

### Configuring the animation

var root: any BlendTreeNode

The first node in a tree of animations.

var name: String

A textual name for the animation.

var bindTarget: BindTarget

A textual name that identifies the particular property that animates.

var blendLayer: Int32

The order in which the framework composites the animation.

var isAdditive: Bool

A Boolean value that indicates whether the animation builds on the current state of the target entity or resets the state before running.

### Timing the animation

var speed: Float

A factor that increases or decreases the animation’s rate of playback.

var delay: TimeInterval

An amount of time that lapses before the animation plays.

var duration: TimeInterval

The total playback time of the animation.

var offset: TimeInterval

The time, in seconds, at which the animation begins within the duration.

var trimDuration: TimeInterval?

An optional duration that overrides the calculated duration.

var trimStart: TimeInterval?

The optional time, in seconds, at which the source animation plays.

var trimEnd: TimeInterval?

The optional time, in seconds, at which the source animation stops.

func trimmed(start: TimeInterval?, end: TimeInterval?, duration: TimeInterval?) -> Self

Edits the animation duration according to the specified time.

### Repeating animation playback

var repeatMode: AnimationRepeatMode

An option that determines how the animation repeats.

var fillMode: AnimationFillMode

An option that determines which data displays outside of the normal duration.

func repeated(count: TimeInterval) -> Self

Repeats an animation the number of times specified by an irrational number.

func repeated(count: Int) -> Self

Repeats an animation the number of times specified by a whole number.

func repeatingForever() -> Self

Repeats the animation infinitely.

### Default Implementations

AnimationDefinition Implementations

## Relationships

### Conforms To

- AnimationDefinition

## See Also

### Blend trees

protocol BlendTreeNode

An interface for a node that’s a member of a blend tree.

struct BlendTreeBlendNode

A source node for an animation that mixes several animations to form a single animation.

struct BlendTreeSourceNode

A blend node that contains an animation.

struct BlendTreeInvalidNode

A blend tree node that’s internal only or sources from an invalid definition.

enum BlendWeight

A numerical representation of the impact an animation has on a scene or entity.

