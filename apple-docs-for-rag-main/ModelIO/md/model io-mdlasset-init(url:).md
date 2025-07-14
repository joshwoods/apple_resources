

- Model I/O
- MDLAsset
-  init(url:) 

Initializer

# init(url:)

Initializes an asset from the file at the specified URL.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(url URL: URL)
```

## Parameters 

`URL`  

A URL specifying the location an asset file.

## Return Value

A new asset object.

## Discussion

Use the canImportFileExtension(_:) method to determine whether Model I/O can import an asset.

## See Also

### Creating an Asset

class func canImportFileExtension(String) -> Bool

Returns a Boolean value that indicates whether the MDLAsset class can read asset data from files with the specified extension.

init(bufferAllocator: (any MDLMeshBufferAllocator)?)

Initializes an empty asset, using the specified buffer allocator.

init(url: URL?, vertexDescriptor: MDLVertexDescriptor?, bufferAllocator: (any MDLMeshBufferAllocator)?)

Initializes an asset from the file at the specified URL, using the specified vertex descriptor and buffer allocator.

init(url: URL, vertexDescriptor: MDLVertexDescriptor?, bufferAllocator: (any MDLMeshBufferAllocator)?, preserveTopology: Bool, error: NSErrorPointer)

Initializes an asset from the file at the specified URL, using the specified options for allocating and transforming data during import.

