

- Metal
- MTLRenderPipelineState
-  supportIndirectCommandBuffers 

Instance Property

# supportIndirectCommandBuffers

A Boolean value that indicates whether the render pipeline supports encoding commands into an indirect command buffer.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+macOS 10.14+tvOS 12.0+visionOS 1.0+

``` source
var supportIndirectCommandBuffers: Bool { get }
```

**Required**

## Discussion

This property gets its value by copying from the supportIndirectCommandBuffers property of the MTLRenderPipelineDescriptor instance as the GPU device creates the pipeline state.

