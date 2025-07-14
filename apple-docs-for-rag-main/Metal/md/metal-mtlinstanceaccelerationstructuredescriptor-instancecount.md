

- Metal
- MTLInstanceAccelerationStructureDescriptor
-  instanceCount 

Instance Property

# instanceCount

The number of instances in the instance descriptor buffer.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var instanceCount: Int { get set }
```

## See Also

### Specifying the List of Instances

var instanceDescriptorBuffer: (any MTLBuffer)?

A buffer that contains descriptions of each instance in the acceleration structure.

var instanceDescriptorBufferOffset: Int

The offset, in bytes, to the descripton of the first instance.

var instanceDescriptorStride: Int

The stride, in bytes, between instance descriptions.

