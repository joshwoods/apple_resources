

- Metal
- MTLDevice
-  makeIOFileHandle(url:compressionMethod:) 

Instance Method

# makeIOFileHandle(url:compressionMethod:)

Creates an input/output file handle instance that represents a compressed file at a URL.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+

``` source
func makeIOFileHandle(
    url: URL,
    compressionMethod: MTLIOCompressionMethod
) throws -> any MTLIOFileHandle
```

**Required**

## Parameters 

`url`  

A location URL to a compressed file in the file system.

`compressionMethod`  

The file’s compression format.

## Return Value

A new MTLIOFileHandle instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

## Discussion

For information about using input/output command queues and file handles, see Resource Loading.

## See Also

### Creating I/O File Handles

func makeIOFileHandle(url: URL) throws -> any MTLIOFileHandle

Creates an input/output file handle instance that represents a file at a URL.

**Required**

func makeIOHandle(url: URL) throws -> any MTLIOFileHandle

Creates an input/output file handle instance that represents a file at a URL.

**Required**

Deprecated

func makeIOHandle(url: URL, compressionMethod: MTLIOCompressionMethod) throws -> any MTLIOFileHandle

Creates an input/output file handle instance that represents a compressed file at a URL.

**Required**

Deprecated

