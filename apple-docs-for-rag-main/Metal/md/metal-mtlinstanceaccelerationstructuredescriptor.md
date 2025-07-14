

- Metal
-  MTLInstanceAccelerationStructureDescriptor 

Class

# MTLInstanceAccelerationStructureDescriptor

A description of an acceleration structure that derives from instances of primitive acceleration structures.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
class MTLInstanceAccelerationStructureDescriptor
```

## Overview

Metal provides acceleration structures with a two-level hierarchy. The bottom layer consists of primitive acceleration structures, which instance acceleration structures in the top level reference.

## Topics

### Specifying the Instance Structures

var instanceDescriptorType: MTLAccelerationStructureInstanceDescriptorType

The format of the instance data in the descriptor buffer.

var instancedAccelerationStructures: [any MTLAccelerationStructure]?

The bottom-level acceleration structures that instances use in the instance acceleration structure .

enum MTLAccelerationStructureInstanceDescriptorType

Options for specifying different kinds of instance types.

### Specifying the List of Instances

var instanceCount: Int

The number of instances in the instance descriptor buffer.

var instanceDescriptorBuffer: (any MTLBuffer)?

A buffer that contains descriptions of each instance in the acceleration structure.

var instanceDescriptorBufferOffset: Int

The offset, in bytes, to the descripton of the first instance.

var instanceDescriptorStride: Int

The stride, in bytes, between instance descriptions.

### Specifying Motion Data

var motionTransformCount: Int

The number of motion transforms in the motion transform buffer.

var motionTransformBuffer: (any MTLBuffer)?

A buffer that contains descriptions of each motion transform in the acceleration structure.

var motionTransformBufferOffset: Int

The offset, in bytes, to the descripton of the first motion transform.

### Instance Properties

var instanceTransformationMatrixLayout: MTLMatrixLayout

var motionTransformStride: Int

var motionTransformType: MTLTransformType

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

class MTLPrimitiveAccelerationStructureDescriptor

A description of an acceleration structure that contains geometry primitives.

protocol MTLAccelerationStructureCommandEncoder

An object for encoding commands that build or refit acceleration structures.

struct MTLAccelerationStructureUsage

Options that describe which tasks you can perform on an acceleration structure and how the system performs those tasks.

struct MTLAccelerationStructureRefitOptions

