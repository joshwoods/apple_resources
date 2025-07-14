

- Metal
- MTLCommandBuffer
-  makeRenderCommandEncoder(descriptor:) 

Instance Method

# makeRenderCommandEncoder(descriptor:)

Creates a render command encoder from a descriptor.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeRenderCommandEncoder(descriptor renderPassDescriptor: MTLRenderPassDescriptor) -> (any MTLRenderCommandEncoder)?
```

**Required**

## Parameters 

`renderPassDescriptor`  

An MTLRenderPassDescriptor instance that configures the MTLRenderCommandEncoder the method returns.

## Discussion

Use an MTLRenderCommandEncoder instance’s methods to set up a single graphics-rendering pass.

