

- Metal
- MTLRenderPassDescriptor
-  visibilityResultBuffer 

Instance Property

# visibilityResultBuffer

A buffer where the GPU writes visibility test results when fragments pass depth and stencil tests.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
var visibilityResultBuffer: (any MTLBuffer)? { get set }
```

## Discussion

When encoding a render pass, you can tell the GPU to record data about fragments that pass depth and stencil tests. Typically, you use visibility testing to track whether a particular piece of geometry is visible in the current frame, so you can omit drawing calls for hidden objects when encoding future frames. This technique is sometimes called *occlusion culling*. You can record separate tests for different pieces of geometry.

Set this property to provide the buffer for the GPU to store visibility results when it executes the render pass. The GPU stores visibility results as 64-bit integers, so you need to reserve `8` bytes for each visibility result that you want to track. After creating the render command encoder, call setVisibilityResultMode(_:offset:) to start each visibility test.

## See Also

### Related Documentation

func setVisibilityResultMode(MTLVisibilityResultMode, offset: Int)

Configures which visibility test the GPU runs and the destination for any results it generates.

**Required**

