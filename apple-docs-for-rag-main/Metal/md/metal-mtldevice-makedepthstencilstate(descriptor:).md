

- Metal
- MTLDevice
-  makeDepthStencilState(descriptor:) 

Instance Method

# makeDepthStencilState(descriptor:)

Creates a depth-stencil state instance.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOSvisionOS 1.0+

``` source
func makeDepthStencilState(descriptor: MTLDepthStencilDescriptor) -> (any MTLDepthStencilState)?
```

**Required**

## Parameters 

`descriptor`  

An MTLDepthStencilDescriptor instance.

## Return Value

A new MTLDepthStencilState instance if the method completed successfully; otherwise `nil`.

