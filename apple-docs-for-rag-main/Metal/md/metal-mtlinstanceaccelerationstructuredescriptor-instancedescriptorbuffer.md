

- Metal
- MTLInstanceAccelerationStructureDescriptor
-  instanceDescriptorBuffer 

Instance Property

# instanceDescriptorBuffer

A buffer that contains descriptions of each instance in the acceleration structure.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var instanceDescriptorBuffer: (any MTLBuffer)? { get set }
```

## Discussion

You must set a buffer before creating the instanced acceleration structure. The buffer must contain a list of instance data structures, each defining the characteristics of an instance. The descriptor’s instanceDescriptorType property determines which memory layout to use for the instance data; see MTLAccelerationStructureInstanceDescriptorType for more information.

## See Also

### Specifying the List of Instances

var instanceCount: Int

The number of instances in the instance descriptor buffer.

var instanceDescriptorBufferOffset: Int

The offset, in bytes, to the descripton of the first instance.

var instanceDescriptorStride: Int

The stride, in bytes, between instance descriptions.

