

- Metal
-  MTLAccelerationStructureInstanceDescriptorType 

Enumeration

# MTLAccelerationStructureInstanceDescriptorType

Options for specifying different kinds of instance types.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
enum MTLAccelerationStructureInstanceDescriptorType
```

## Topics

### Specifying the Instance Descriptor Type

case `default`

An option specifying that the instance uses the default characteristics.

case userID

An option specifying that the instance contains a user identifier.

case motion

An option specifying that the instance contains motion data.

case indirect

An option that enables using an instance descriptor memory layout that the GPU can populate.

case indirectMotion

An option specifying that the instance contains motion data, and enables using an instance descriptor memory layout that the GPU can populate.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Specifying the Instance Structures

var instanceDescriptorType: MTLAccelerationStructureInstanceDescriptorType

The format of the instance data in the descriptor buffer.

var instancedAccelerationStructures: [any MTLAccelerationStructure]?

The bottom-level acceleration structures that instances use in the instance acceleration structure .

