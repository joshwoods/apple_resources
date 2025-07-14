

- Metal
- MTLInstanceAccelerationStructureDescriptor
-  instanceDescriptorType 

Instance Property

# instanceDescriptorType

The format of the instance data in the descriptor buffer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 16.0+visionOS 1.0+

``` source
var instanceDescriptorType: MTLAccelerationStructureInstanceDescriptorType { get set }
```

## See Also

### Related Documentation

var instanceDescriptorBuffer: (any MTLBuffer)?

A buffer that contains descriptions of each instance in the acceleration structure.

### Specifying the Instance Structures

var instancedAccelerationStructures: [any MTLAccelerationStructure]?

The bottom-level acceleration structures that instances use in the instance acceleration structure .

enum MTLAccelerationStructureInstanceDescriptorType

Options for specifying different kinds of instance types.

