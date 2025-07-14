

- MetalKit
-  MTKModelIOVertexFormatFromMetal(\_:) 

Function

# MTKModelIOVertexFormatFromMetal(\_:)

Returns a converted Model I/O vertex format.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func MTKModelIOVertexFormatFromMetal(_ vertexFormat: MTLVertexFormat) -> MDLVertexFormat
```

## Parameters 

`vertexFormat`  

A Metal vertex format to convert from.

## Return Value

A Model I/O vertex format value.

## Discussion

This function returns MDLVertexFormat.invalid if no matching MDLVertexFormat exists.

## See Also

### Converting Between Model I/O and Metal Vertex Formats

func MTKMetalVertexFormatFromModelIO(MDLVertexFormat) -> MTLVertexFormat

Returns a converted Metal vertex format.

