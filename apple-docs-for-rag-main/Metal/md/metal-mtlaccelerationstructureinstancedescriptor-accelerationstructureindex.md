

- Metal
- MTLAccelerationStructureInstanceDescriptor
-  accelerationStructureIndex 

Instance Property

# accelerationStructureIndex

The index of the acceleration structure to use for the instance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
var accelerationStructureIndex: UInt32
```

## Discussion

This index refers to a bottom-level instance in the instancedAccelerationStructures of the MTLInstanceAccelerationStructureDescriptor that you use to create the new instance acceleration structure.

## See Also

### Related Documentation

var instancedAccelerationStructures: [any MTLAccelerationStructure]?

The bottom-level acceleration structures that instances use in the instance acceleration structure .

