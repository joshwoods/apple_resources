

- MetalKit
-  MTKModelIOVertexDescriptorFromMetal(\_:) 

Function

# MTKModelIOVertexDescriptorFromMetal(\_:)

Returns a partially converted Model I/O vertex descriptor.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func MTKModelIOVertexDescriptorFromMetal(_ metalDescriptor: MTLVertexDescriptor) -> MDLVertexDescriptor
```

## Parameters 

`metalDescriptor`  

A Metal vertex descriptor to convert from.

## Return Value

A Model I/O vertex descriptor object.

## Discussion

This function is equivalent to the MTKModelIOVertexDescriptorFromMetalWithError function, but does not report errors.

## See Also

### Converting Between Model I/O and Metal Vertex Descriptors

func MTKMetalVertexDescriptorFromModelIO(MDLVertexDescriptor) -> MTLVertexDescriptor?

Returns a partially converted Metal vertex descriptor.

