

- Model I/O
- MDLAsset
-  init(url:vertexDescriptor:bufferAllocator:) 

Initializer

# init(url:vertexDescriptor:bufferAllocator:)

Initializes an asset from the file at the specified URL, using the specified vertex descriptor and buffer allocator.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    url URL: URL?,
    vertexDescriptor: MDLVertexDescriptor?,
    bufferAllocator: (any MDLMeshBufferAllocator)?
)
```

## Parameters 

`URL`  

A URL specifying the location an asset file.

`vertexDescriptor`  

An object describing the vertex data format to be loaded from the asset, or `nil` to use the asset’s vertex buffers as found in the file.

`bufferAllocator`  

The allocator object to use for loading mesh data from the asset, or `nil` to use a default allocator.

## Return Value

A new asset object.

## Discussion

Using this initializer is equivalent to using the init(url:vertexDescriptor:bufferAllocator:preserveTopology:error:) initializer, passing false for the `preserveTopology` parameter and ignoring errors.

## See Also

### Creating an Asset

class func canImportFileExtension(String) -> Bool

Returns a Boolean value that indicates whether the MDLAsset class can read asset data from files with the specified extension.

init(url: URL)

Initializes an asset from the file at the specified URL.

init(bufferAllocator: (any MDLMeshBufferAllocator)?)

Initializes an empty asset, using the specified buffer allocator.

init(url: URL, vertexDescriptor: MDLVertexDescriptor?, bufferAllocator: (any MDLMeshBufferAllocator)?, preserveTopology: Bool, error: NSErrorPointer)

Initializes an asset from the file at the specified URL, using the specified options for allocating and transforming data during import.

