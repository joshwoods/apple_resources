

- Metal
- MTLInstanceAccelerationStructureDescriptor
-  instanceDescriptorStride 

Instance Property

# instanceDescriptorStride

The stride, in bytes, between instance descriptions.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 16.0+visionOS 1.0+

``` source
var instanceDescriptorStride: Int { get set }
```

## Discussion

The stride must be at least 64 bytes and must be a multiple of 4 bytes. Defaults to 64 bytes.

## See Also

### Specifying the List of Instances

var instanceCount: Int

The number of instances in the instance descriptor buffer.

var instanceDescriptorBuffer: (any MTLBuffer)?

A buffer that contains descriptions of each instance in the acceleration structure.

var instanceDescriptorBufferOffset: Int

The offset, in bytes, to the descripton of the first instance.

