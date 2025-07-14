

- Metal
-  MTLIndirectInstanceAccelerationStructureDescriptor 

Class

# MTLIndirectInstanceAccelerationStructureDescriptor

A description of an acceleration structure that Metal derives from instances of primitive acceleration structures that the GPU can populate.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
class MTLIndirectInstanceAccelerationStructureDescriptor
```

## Topics

### Instance Properties

var instanceCountBuffer: (any MTLBuffer)?

var instanceCountBufferOffset: Int

var instanceDescriptorBuffer: (any MTLBuffer)?

var instanceDescriptorBufferOffset: Int

var instanceDescriptorStride: Int

var instanceDescriptorType: MTLAccelerationStructureInstanceDescriptorType

var instanceTransformationMatrixLayout: MTLMatrixLayout

var maxInstanceCount: Int

var maxMotionTransformCount: Int

var motionTransformBuffer: (any MTLBuffer)?

var motionTransformBufferOffset: Int

var motionTransformCountBuffer: (any MTLBuffer)?

var motionTransformCountBufferOffset: Int

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

### Instance Descriptors

struct MTLAccelerationStructureInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure.

struct MTLAccelerationStructureUserIDInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure, with the instance including a user identifier for the instance.

struct MTLAccelerationStructureMotionInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure, with the instance including a user identifier and motion data for the instance.

struct MTLAccelerationStructureInstanceOptions

Options for adjusting the behavior of an instanced acceleration structure.

struct MTLIndirectAccelerationStructureInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure that the GPU can populate.

struct MTLIndirectAccelerationStructureMotionInstanceDescriptor

A description of an instance in an acceleration structure that the GPU can populate, with motion data for the instance.

