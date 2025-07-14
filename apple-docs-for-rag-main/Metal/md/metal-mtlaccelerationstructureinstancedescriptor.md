

- Metal
-  MTLAccelerationStructureInstanceDescriptor 

Structure

# MTLAccelerationStructureInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
struct MTLAccelerationStructureInstanceDescriptor
```

## Topics

### Creating an Instance Descriptor

init()

Creates a default acceleration structure instance.

init(transformationMatrix: MTLPackedFloat4x3, options: MTLAccelerationStructureInstanceOptions, mask: UInt32, intersectionFunctionTableOffset: UInt32, accelerationStructureIndex: UInt32)

Creates a new acceleration structure instance.

### Specifying the Instance

var accelerationStructureIndex: UInt32

The index of the acceleration structure to use for the instance.

### Specifying the Instance Transform

var transformationMatrix: MTLPackedFloat4x3

The transform for placing and orienting the instance in the scene.

### Customizing Intersection and Hit Tests for the Instance

var intersectionFunctionTableOffset: UInt32

An offset for determining which function in the intersection function table Metal needs to call when testing a ray against the instance.

var options: MTLAccelerationStructureInstanceOptions

The options for the instance.

var mask: UInt32

A mask to use for the instance when testing a ray against the geometry.

## Relationships

### Conforms To

- Sendable

## See Also

### Instance Descriptors

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

struct MTLIndirectAccelerationStructureMotionInstanceDescriptor

A description of an instance in an acceleration structure that the GPU can populate, with motion data for the instance.

