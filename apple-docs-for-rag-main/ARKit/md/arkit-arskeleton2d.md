

- ARKit
-  ARSkeleton2D 

Class

# ARSkeleton2D

An object that describes the locations of a body’s joints in the camera feed.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
class ARSkeleton2D
```

## Overview

ARSkeleton2D provides you with a 2D body’s joints in a flat hierarchy so you can access them efficiently. The joint locations are normalized within the range \[0..1\] in the coordinate space of the current frame’s camera image, where 0 is the upper left, and 1 is the bottom right.

To access a skeleton’s joints by name, you use landmarkForJointNamed:. To access a named joint by index (for example, for performance reasons), you query the definition for the named joint index using index(for:), then access jointLandmarks using the resulting index.

## Topics

### Getting Joint Landmarks

var jointLandmarks: [simd_float2]

The joint landmarks in normalized coordinates.

func landmark(for: ARSkeleton.JointName) -> simd_float2?

Returns the location of a joint with a given name.

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

class ARSkeleton3D

The skeleton of a human body that ARKit tracks in 3D space.

class ARSkeleton

The interface for the skeleton of a tracked body.

class ARSkeletonDefinition

The hierarchy of joints and their names.

