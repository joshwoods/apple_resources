

- MetalKit
-  MTKMetalVertexDescriptorFromModelIO(\_:) 

Function

# MTKMetalVertexDescriptorFromModelIO(\_:)

Returns a partially converted Metal vertex descriptor.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func MTKMetalVertexDescriptorFromModelIO(_ modelIODescriptor: MDLVertexDescriptor) -> MTLVertexDescriptor?
```

## Return Value

A Metal vertex descriptor object.

## Discussion

This function is equivalent to the MTKMetalVertexDescriptorFromModelIOWithError function, but does not report errors.

## See Also

### Converting Between Model I/O and Metal Vertex Descriptors

func MTKModelIOVertexDescriptorFromMetal(MTLVertexDescriptor) -> MDLVertexDescriptor

Returns a partially converted Model I/O vertex descriptor.

