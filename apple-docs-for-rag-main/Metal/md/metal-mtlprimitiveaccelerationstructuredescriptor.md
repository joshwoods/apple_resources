

- Metal
-  MTLPrimitiveAccelerationStructureDescriptor 

Class

# MTLPrimitiveAccelerationStructureDescriptor

A description of an acceleration structure that contains geometry primitives.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLPrimitiveAccelerationStructureDescriptor
```

## Overview

Metal provides acceleration structures with a two-level hierarchy. The bottom layer consists of primitive acceleration structures, which instance acceleration structures in the top level reference.

## Topics

### Specifying Geometry

var geometryDescriptors: [MTLAccelerationStructureGeometryDescriptor]?

An array that contains the individual pieces of geometry that compose the acceleration structure.

### Specifying Motion Behavior

var motionKeyframeCount: Int

The number of keyframes in the geometry data.

var motionStartTime: Float

The start time for the range of motion that the keyframe data describes.

var motionEndTime: Float

The end time for the range of motion that the keyframe data describes.

var motionStartBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps before the start time.

var motionEndBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps after the end time.

enum MTLMotionBorderMode

Options for specifying how the acceleration structure handles timestamps that are outside the specified range.

## Relationships

### Inherits From

- MTLAccelerationStructureDescriptor

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Acceleration Structures

Improving Ray-Tracing Data Access Using Per-Primitive Data

Simplify data access and improve GPU utilization by storing custom primitive data directly in the acceleration structure.

protocol MTLAccelerationStructure

A collection of model data for GPU-accelerated intersection of rays with the model.

class MTLAccelerationStructureDescriptor

A base class for classes that define the configuration for a new acceleration structure.

class MTLInstanceAccelerationStructureDescriptor

A description of an acceleration structure that derives from instances of primitive acceleration structures.

protocol MTLAccelerationStructureCommandEncoder

An object for encoding commands that build or refit acceleration structures.

struct MTLAccelerationStructureUsage

Options that describe which tasks you can perform on an acceleration structure and how the system performs those tasks.

struct MTLAccelerationStructureRefitOptions

