

- Metal
-  MTLAccelerationStructureInstanceOptions 

Structure

# MTLAccelerationStructureInstanceOptions

Options for adjusting the behavior of an instanced acceleration structure.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
struct MTLAccelerationStructureInstanceOptions
```

## Topics

### Creating Instance Flags

init(rawValue: UInt32)

Creates new usage options from a raw integer value.

### Usage Options

static var disableTriangleCulling: MTLAccelerationStructureInstanceOptions

An option that turns off culling for this instance if ray intersector has culling enabled.

static var triangleFrontFacingWindingCounterClockwise: MTLAccelerationStructureInstanceOptions

Specifies that the instance specifies front facing triangles in counter-clockwise order.

static var opaque: MTLAccelerationStructureInstanceOptions

Specifies that intersectors should treat the instance as opaque.

static var nonOpaque: MTLAccelerationStructureInstanceOptions

Specifies that intersectors should treat the instance as non-opaque.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Instance Descriptors

struct MTLAccelerationStructureInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure.

struct MTLAccelerationStructureUserIDInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure, with the instance including a user identifier for the instance.

struct MTLAccelerationStructureMotionInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure, with the instance including a user identifier and motion data for the instance.

class MTLIndirectInstanceAccelerationStructureDescriptor

A description of an acceleration structure that Metal derives from instances of primitive acceleration structures that the GPU can populate.

struct MTLIndirectAccelerationStructureInstanceDescriptor

A description of an instance in an instanced geometry acceleration structure that the GPU can populate.

struct MTLIndirectAccelerationStructureMotionInstanceDescriptor

A description of an instance in an acceleration structure that the GPU can populate, with motion data for the instance.

