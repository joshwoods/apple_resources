

- Metal
- MTLCommandBuffer
-  makeParallelRenderCommandEncoder(descriptor:) 

Instance Method

# makeParallelRenderCommandEncoder(descriptor:)

Creates a parallel render command encoder from a descriptor.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeParallelRenderCommandEncoder(descriptor renderPassDescriptor: MTLRenderPassDescriptor) -> (any MTLParallelRenderCommandEncoder)?
```

**Required**

## Parameters 

`renderPassDescriptor`  

An MTLRenderPassDescriptor instance that configures the MTLParallelRenderCommandEncoder the method returns.

## Discussion

An MTLParallelRenderCommandEncoder instance can create multiple, independent render command encoders that contribute to the same render pass on different threads.

