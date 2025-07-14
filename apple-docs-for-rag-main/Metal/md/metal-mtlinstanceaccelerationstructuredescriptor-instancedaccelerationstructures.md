

- Metal
- MTLInstanceAccelerationStructureDescriptor
-  instancedAccelerationStructures 

Instance Property

# instancedAccelerationStructures

The bottom-level acceleration structures that instances use in the instance acceleration structure .

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var instancedAccelerationStructures: [any MTLAccelerationStructure]? { get set }
```

## Discussion

Each instance in the instance descriptor buffer has an index into this array, specifying which acceleration structure to use for that instance.

## See Also

### Related Documentation

var accelerationStructureIndex: UInt32

The index of the acceleration structure to use for the instance.

### Specifying the Instance Structures

var instanceDescriptorType: MTLAccelerationStructureInstanceDescriptorType

The format of the instance data in the descriptor buffer.

enum MTLAccelerationStructureInstanceDescriptorType

Options for specifying different kinds of instance types.

