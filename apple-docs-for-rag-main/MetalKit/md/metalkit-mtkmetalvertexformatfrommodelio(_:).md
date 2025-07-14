

- MetalKit
-  MTKMetalVertexFormatFromModelIO(\_:) 

Function

# MTKMetalVertexFormatFromModelIO(\_:)

Returns a converted Metal vertex format.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func MTKMetalVertexFormatFromModelIO(_ vertexFormat: MDLVertexFormat) -> MTLVertexFormat
```

## Parameters 

`vertexFormat`  

A Model I/O vertex format to convert from.

## Return Value

A Metal vertex format value.

## Discussion

This function returns MTLVertexFormat.invalid if no matching MTLVertexFormat exists.

## See Also

### Converting Between Model I/O and Metal Vertex Formats

func MTKModelIOVertexFormatFromMetal(MTLVertexFormat) -> MDLVertexFormat

Returns a converted Model I/O vertex format.

