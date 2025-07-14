

- Model I/O
- MDLAsset
-  init(bufferAllocator:) 

Initializer

# init(bufferAllocator:)

Initializes an empty asset, using the specified buffer allocator.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(bufferAllocator: (any MDLMeshBufferAllocator)?)
```

## Parameters 

`bufferAllocator`  

The allocator object to use for loading or creating mesh data associated with the asset, or `nil` to use a default allocator.

## Return Value

A new asset object.

## Discussion

Use this initializer when you want to programmatically populate an asset with content (for example, for use in exporting to a file) while controlling the allocation of mesh data buffers associated with the asset. For example, to use the MetalKit framework for loading vertex data into GPU buffers for rendering using Metal, pass a MTKMeshBufferAllocator object for the `bufferAllocator` parameter.

## See Also

### Creating an Asset

class func canImportFileExtension(String) -> Bool

Returns a Boolean value that indicates whether the MDLAsset class can read asset data from files with the specified extension.

init(url: URL)

Initializes an asset from the file at the specified URL.

init(url: URL?, vertexDescriptor: MDLVertexDescriptor?, bufferAllocator: (any MDLMeshBufferAllocator)?)

Initializes an asset from the file at the specified URL, using the specified vertex descriptor and buffer allocator.

init(url: URL, vertexDescriptor: MDLVertexDescriptor?, bufferAllocator: (any MDLMeshBufferAllocator)?, preserveTopology: Bool, error: NSErrorPointer)

Initializes an asset from the file at the specified URL, using the specified options for allocating and transforming data during import.

