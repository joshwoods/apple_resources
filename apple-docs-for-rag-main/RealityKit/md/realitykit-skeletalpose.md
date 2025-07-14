

- RealityKit
-  SkeletalPose 

Structure

# SkeletalPose

A container that holds the position and orientation of each joint in a single animation skeleton.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
struct SkeletalPose
```

## Overview

Each index in jointNames directly corresponds to the same index in jointTransforms, linking each joint name to its respective transform.

## Topics

### Initializers

init(id: SkeletalPose.ID, from: MeshResource.Skeleton)

Creates a skeletal pose from the rest pose of the model skeleton.

init(id: SkeletalPose.ID, joints: [(String, JointTransforms.Element)])

Creates a pose for the joint name and transformation pairs.

### Instance Properties

var id: SkeletalPose.ID

The unique identifier of the pose.

var jointNames: [String]

The names of the joints in the pose in specific order.

var jointTransforms: JointTransforms

The transformations of the joints in the pose.

### Subscripts

subscript(String) -> Transform?

Accesses a pose transformation using the index of the joint name.

### Type Aliases

typealias ID

A type representing the stable identity of the entity associated with an instance.

## Relationships

### Conforms To

- Identifiable

## See Also

### Skeletons

struct SkeletalPosesComponent

A component that exposes the collection of named animation skeletal poses.

typealias ID

A type representing the stable identity of the entity associated with an instance.

struct SkeletalPoseSet

A collection of named skeletal poses.

typealias Element

A type representing the sequence’s elements.

