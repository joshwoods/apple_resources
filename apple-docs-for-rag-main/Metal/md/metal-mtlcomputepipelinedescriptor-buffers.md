

- Metal
- MTLComputePipelineDescriptor
-  buffers 

Instance Property

# buffers

The buffer mutability options to apply to the next kernel call.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
var buffers: MTLPipelineBufferDescriptorArray { get }
```

## Discussion

This property holds an array of MTLPipelineBufferDescriptor instances, where each index corresponds to the same entry in the buffer argument table.

Metal can perform additional optimizations if you guarantee that neither the CPU nor the GPU modify a buffer’s contents after set in a function’s argument table and before its command buffer completes. Use immutable buffers as much as possible, for either regular buffers or argument buffers.

```
// Compute setup.
// Set mutability for buffer at index 9.
MTLComputePipelineDescriptor *computeDescriptor = [MTLComputePipelineDescriptor new];
computeDescriptor.buffers[9].mutability = MTLMutabilityImmutable;
// Compute pass.
// Set immutable buffer at index 9.
id  computeEncoder = [_commandBuffer computeCommandEncoder];
[computeEncoder setBuffer:_buffer offset:0 atIndex:9];
```

