

- Metal
-  MTLIndirectAccelerationStructureMotionInstanceDescriptor 

Structure

# MTLIndirectAccelerationStructureMotionInstanceDescriptor

A description of an instance in an acceleration structure that the GPU can populate, with motion data for the instance.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
struct MTLIndirectAccelerationStructureMotionInstanceDescriptor
```

## Topics

### Specifying the Instance

var accelerationStructureID: MTLResourceID

The acceleration resource handle to use for this instance.

### Specifying Motion Data

var motionStartTime: Float

The start time of the motion instance.

var motionStartBorderMode: MTLMotionBorderMode

The motion border mode describing what happens if Metal samples the acceleration structure before the motion start time.

var motionEndTime: Float

The end time of the motion instance.

var motionEndBorderMode: MTLMotionBorderMode

The motion border mode describing what happens if Metal samples the acceleration structure after the motion end time.

var motionTransformsCount: UInt32

The number of motion transforms belonging to the motion instance.

var motionTransformsStartIndex: UInt32

The index of the first set of transforms describing one keyframe of the animation.

### Specifying the User Identifier

var userID: UInt32

A user-assigned ID to help identify the instance.

### Initializers

init()

Creates a default indirect acceleration structure instance.

init(options: MTLAccelerationStructureInstanceOptions, mask: UInt32, intersectionFunctionTableOffset: UInt32, userID: UInt32, accelerationStructureID: MTLResourceID, motionTransformsStartIndex: UInt32, motionTransformsCount: UInt32, motionStartBorderMode: MTLMotionBorderMode, motionEndBorderMode: MTLMotionBorderMode, motionStartTime: Float, motionEndTime: Float)

Creates an indirect acceleration structure instance.

### Instance Properties

var intersectionFunctionTableOffset: UInt32

An offset for determining which function in the intersection function table Metal calls when testing a ray against the instance.

var mask: UInt32

An instance mask to ignore geometry during ray tracing.

var options: MTLAccelerationStructureInstanceOptions

The options for this instance.

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

struct MTLAccelerationStructureMotionInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure, with the instance including a user identifier and motion data for the instance.

struct MTLAccelerationStructureInstanceOptions

Options for adjusting the behavior of an instanced acceleration structure.

class MTLIndirectInstanceAccelerationStructureDescriptor

A description of an acceleration structure that Metal derives from instances of primitive acceleration structures that the GPU can populate.

struct MTLIndirectAccelerationStructureInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure that the GPU can populate.

