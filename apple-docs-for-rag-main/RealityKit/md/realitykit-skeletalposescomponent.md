

- RealityKit
-  SkeletalPosesComponent 

Structure

# SkeletalPosesComponent

A component that exposes the collection of named animation skeletal poses.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct SkeletalPosesComponent
```

## Overview

Use the entity’s skeletal poses to either read the pose evaluated from animations bound to BindTarget.jointTransforms and BindTarget.skeletalPose(_:), or write your own pose to animate the skeletal model.

### Setting updated value on an entity

When an updated SkeletalPose is set on an entity as part of this component, these rules are followed:

- If jointNames is reordered, following animation updated will match the new order.

- If jointTransforms contains more elements than jointNames, the extra transformations are ignored.

- If jointTransforms contains less elements than jointNames, the extra joint transformations are not updated.

You can use poses’s default accessor for the same skeletal pose as exposed by jointNames and jointTransforms. The access trough the component allows the reordering, addition and removal of joints from the default pose.

## Topics

### Initializers

init(poses: [SkeletalPose])

Creates a component value with the provided poses.

### Instance Properties

var poses: SkeletalPoseSet

The collection of the skeletal poses for a single entity.

### Default Implementations

Component Implementations

## Relationships

### Conforms To

- Component

## See Also

### Skeletons

struct SkeletalPose

A container that holds the position and orientation of each joint in a single animation skeleton.

typealias ID

A type representing the stable identity of the entity associated with an instance.

struct SkeletalPoseSet

A collection of named skeletal poses.

typealias Element

A type representing the sequence’s elements.

