

- Metal
-  MTLAccelerationStructureMotionInstanceDescriptor 

Structure

# MTLAccelerationStructureMotionInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure, with the instance including a user identifier and motion data for the instance.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
struct MTLAccelerationStructureMotionInstanceDescriptor
```

## Topics

### Creating an Instance Descriptor

init()

Creates a default acceleration structure instance.

init(options: MTLAccelerationStructureInstanceOptions, mask: UInt32, intersectionFunctionTableOffset: UInt32, accelerationStructureIndex: UInt32, userID: UInt32, motionTransformsStartIndex: UInt32, motionTransformsCount: UInt32, motionStartBorderMode: MTLMotionBorderMode, motionEndBorderMode: MTLMotionBorderMode, motionStartTime: Float, motionEndTime: Float)

Creates a new acceleration structure instance.

### Specifying the Instance

var accelerationStructureIndex: UInt32

The index of the acceleration structure to use for this instance.

### Specifying Motion Data

var motionStartTime: Float

The start time for the range of motion described by the keyframe data.

var motionEndTime: Float

The end time for the range of motion described by the keyframe data.

var motionStartBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps before the start time.

var motionEndBorderMode: MTLMotionBorderMode

The mode to use when handling timestamps after the end time.

var motionTransformsStartIndex: UInt32

The index for the instance’s first keyframe motion data.

var motionTransformsCount: UInt32

The number of keyframes for this instance.

### Customizing Intersection and Hit Tests for the Instance

var intersectionFunctionTableOffset: UInt32

An offset used to determine which function in the intersection function table Metal should call when testing a ray against this instance.

var options: MTLAccelerationStructureInstanceOptions

The options for this instance.

var mask: UInt32

A mask used for this instance when testing a ray against the geometry.

### Specifying the User Identifier

var userID: UInt32

The user identifier for the instance.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Instance Descriptors

struct MTLAccelerationStructureInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure.

struct MTLAccelerationStructureUserIDInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure, with the instance including a user identifier for the instance.

struct MTLAccelerationStructureInstanceOptions

Options for adjusting the behavior of an instanced acceleration structure.

class MTLIndirectInstanceAccelerationStructureDescriptor

A description of an acceleration structure that Metal derives from instances of primitive acceleration structures that the GPU can populate.

struct MTLIndirectAccelerationStructureInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure that the GPU can populate.

struct MTLIndirectAccelerationStructureMotionInstanceDescriptor

A description of an instance in an acceleration structure that the GPU can populate, with motion data for the instance.

