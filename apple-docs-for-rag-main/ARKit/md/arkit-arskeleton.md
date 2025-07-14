

- ARKit
-  ARSkeleton 

Class

# ARSkeleton

The interface for the skeleton of a tracked body.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARSkeleton
```

## Overview

As a collection of joints, this protocol describes the state of a human body whose movements ARKit can track.

The ARSkeleton3D subclass provides you with the position of a tracked body’s joints in 3D space, specifically with its jointLocalTransforms and jointModelTransforms properties.

The ARSkeleton2D subclass provides you with the position of a tracked body’s joints in 2D space, by way of its jointLandmarks property.

## Topics

### Getting Joint Information

var definition: ARSkeletonDefinition

The particular configuration of joints that define a body’s current state.

func isJointTracked(Int) -> Bool

Tells you whether ARKit tracks a joint at a particular index.

struct JointName

A name identifier for a joint.

## Relationships

### Inherits From

- NSObject

### Inherited By

- ARSkeleton2D
- ARSkeleton3D

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

class ARSkeletonDefinition

The hierarchy of joints and their names.

