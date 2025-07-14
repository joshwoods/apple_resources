

- Metal
- MTLInstanceAccelerationStructureDescriptor
-  instanceDescriptorBufferOffset 

Instance Property

# instanceDescriptorBufferOffset

The offset, in bytes, to the descripton of the first instance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var instanceDescriptorBufferOffset: Int { get set }
```

## Discussion

Specify an offset that is a multiple of 4 bytes and a multiple of the platform’s buffer offset alignment.

## See Also

### Specifying the List of Instances

var instanceCount: Int

The number of instances in the instance descriptor buffer.

var instanceDescriptorBuffer: (any MTLBuffer)?

A buffer that contains descriptions of each instance in the acceleration structure.

var instanceDescriptorStride: Int

The stride, in bytes, between instance descriptions.

