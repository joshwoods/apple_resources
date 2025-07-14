

- ARKit
-  ARSkeleton3D 

Class

# ARSkeleton3D

The skeleton of a human body that ARKit tracks in 3D space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARSkeleton3D
```

## Overview

An ARBodyAnchor contains one instance of this ARSkeleton subclass to provide its joint positions in 3D space. The jointLocalTransforms property describes a joint’s 3D offset from its parent joint. The jointModelTransforms property describes a joint’s 3D offset from the body anchor’s transform.

## Topics

### Getting a Joint’s Pose

var jointLocalTransforms: [simd_float4x4]

The local space transforms for each joint.

var jointModelTransforms: [simd_float4x4]

The model space transforms for each joint.

func localTransform(for: ARSkeleton.JointName) -> simd_float4x4?

Returns the local transform for a joint with a given name.

func modelTransform(for: ARSkeleton.JointName) -> simd_float4x4?

Returns the model transform for a joint with a given name.

## Relationships

### Inherits From

- ARSkeleton

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Body Data

Capturing Body Motion in 3D

Track a person in the physical environment and visualize their motion by applying the same body movements to a virtual character.

class ARBody2D

The screen-space representation of a person ARKit recognizes in the camera feed.

class ARSkeleton2D

An object that describes the locations of a body’s joints in the camera feed.

class ARSkeleton

The interface for the skeleton of a tracked body.

class ARSkeletonDefinition

The hierarchy of joints and their names.

