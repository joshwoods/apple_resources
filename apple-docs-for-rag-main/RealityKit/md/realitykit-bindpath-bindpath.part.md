

- RealityKit
- BindPath
-  BindPath.Part 

Enumeration

# BindPath.Part

An individual piece of a larger path that refers to the target of an animation.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS

``` source
enum Part
```

## Overview

Path-based instances of bindTarget, or those identified by the BindTarget.path(_:) call, consist of one or more components identified by these enumeration options.

For example, the succession of BindPath.Part calls in the following code results in a path with a parts array that contains three components: `entityA`, `entityB`, and `myInt`.

```
let target3: BindTarget = .entity("entityA").entity("entityB").parameter("myInt")
```

## Topics

### Choosing the path component

case anchorEntity(String)

A path component for the scene’s anchor entity.

case entity(String)

A path component for a nested entity.

case jointTransforms

A path component to animate joint transforms.

case parameter(String)

A path component to animate a named parameter.

case scene(String)

A path component for a nested scene.

case transform

A path component to animate a transform.

### Comparing bind parts

static func == (BindPath.Part, BindPath.Part) -> Bool

Returns a Boolean value that indicates whether two components of a bind path are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Enumeration Cases

case billboardBlendFactor

case blendShapeWeights

An option the entity’s blend shape weights animate. Requires that the entity has a BlendShapeWeightsComponent. Can be indexed by blend shape index or by blend shape name. Default is by index 0.

case blendShapeWeightsAtIndex(Int)

case blendShapeWeightsWithID(BlendShapeWeightsData.ID)

case ikConstraintLookAtTarget(IKComponent.Constraint.ID)

A path component to an IK solver’s constraint target look at position.

case ikConstraintTarget(IKComponent.Constraint.ID)

A path component to an IK solver’s constraint target transform.

case ikSolver(IKComponent.Solver.ID?)

A path component to an IK solver instance.

case material(Int)

A path component to animate a material property.

case materialParameter(String)

A path component to name a material parameter to animate

case opacity

An path component to animate an opacity. Requires that the entity has an OpacityComponent

case skeletalPose(SkeletalPose.ID)

### Default Implementations

Equatable Implementations

## Relationships

### Conforms To

- Equatable

## See Also

### Composing a property identifier

var parts: [BindPath.Part]

An array of the individual components of a complete bind path.

