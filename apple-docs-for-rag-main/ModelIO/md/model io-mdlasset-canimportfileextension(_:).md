

- Model I/O
- MDLAsset
-  canImportFileExtension(\_:) 

Type Method

# canImportFileExtension(\_:)

Returns a Boolean value that indicates whether the MDLAsset class can read asset data from files with the specified extension.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
class func canImportFileExtension(_ extension: String) -> Bool
```

## Parameters 

`extension`  

The filename extension identifying an asset file format.

## Return Value

true if the MDLAsset class can read asset data from files with the specified extension; otherwise, false.

## Discussion

If this method returns true, you can use the init(url:) or init(url:vertexDescriptor:bufferAllocator:) initializer to import an asset with the specified filename extension.

The set of supported extensions and formats includes:

`.abc`  
Alembic

`.usd`, `.usda`, `.usdc`  
Universal Scene Description

`.usdz`  
Universal Scene Description (Mobile)

`.ply`  
Polygon

`.obj`  
Wavefront Object

`.stl`  
Standard Tessellation Language

Additional formats may be supported as well.

## See Also

### Creating an Asset

init(url: URL)

Initializes an asset from the file at the specified URL.

init(bufferAllocator: (any MDLMeshBufferAllocator)?)

Initializes an empty asset, using the specified buffer allocator.

init(url: URL?, vertexDescriptor: MDLVertexDescriptor?, bufferAllocator: (any MDLMeshBufferAllocator)?)

Initializes an asset from the file at the specified URL, using the specified vertex descriptor and buffer allocator.

init(url: URL, vertexDescriptor: MDLVertexDescriptor?, bufferAllocator: (any MDLMeshBufferAllocator)?, preserveTopology: Bool, error: NSErrorPointer)

Initializes an asset from the file at the specified URL, using the specified options for allocating and transforming data during import.

