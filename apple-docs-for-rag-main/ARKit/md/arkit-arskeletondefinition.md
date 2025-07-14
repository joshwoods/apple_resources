

- ARKit
-  ARSkeletonDefinition 

Class

# ARSkeletonDefinition

The hierarchy of joints and their names.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARSkeletonDefinition
```

## Overview

A skeleton definition establishes the relationship of joints that make up a 3D or 2D body’s skeleton, in which joints connect to other joints to compose a single skeleton in a parent-child hierarchy. Use parentIndices to identify the hierarchy for a given skeleton definition.

ARKit names particular joints that are crucial to body tracking. You can access named joints by calling indexForJointName: and passing in one of the available jointNames identifiers.

## Topics

### Locating in the Physical Environment

var neutralBodySkeleton3D: ARSkeleton3D?

The 3D skeleton in neutral pose.

class var defaultBody3D: ARSkeletonDefinition

The default skeleton definition for bodies defined in 3D.

### Locating in Screen Space

class var defaultBody2D: ARSkeletonDefinition

The default skeleton definition for bodies defined in 2D.

### Getting Joint Information

var jointNames: [String]

A collection of unique joint names.

var jointCount: Int

The skeleton’s total number of joints.

func index(for: ARSkeleton.JointName) -> Int

Returns the index for a given joint identifier.

var parentIndices: [Int]

The parent index for each joint.

## Relationships

### Inherits From

- NSObject

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

class ARSkeleton3D

The skeleton of a human body that ARKit tracks in 3D space.

class ARSkeleton2D

An object that describes the locations of a body’s joints in the camera feed.

class ARSkeleton

The interface for the skeleton of a tracked body.

