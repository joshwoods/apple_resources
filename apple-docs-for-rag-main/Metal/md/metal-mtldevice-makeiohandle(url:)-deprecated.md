

- Metal
- MTLDevice
-  makeIOHandle(url:) Deprecated

Instance Method

# makeIOHandle(url:)

Creates an input/output file handle instance that represents a file at a URL.

iOS 16.0–17.0DeprecatediPadOS 16.0–17.0DeprecatedMac Catalyst 16.0–17.0DeprecatedmacOS 13.0–14.0DeprecatedtvOS 16.0–17.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func makeIOHandle(url: URL) throws -> any MTLIOFileHandle
```

**Required**

Deprecated

Use makeIOFileHandle(url:) instead.

## Parameters 

`url`  

The URL to a resource file in the file system.

## Return Value

A new MTLIOFileHandle instance if the method completes successfully; otherwise Swift throws an error and Objective-C returns `nil`.

## Discussion

For information about using input/output command queues and file handles, see Resource Loading.

## See Also

### Creating I/O File Handles

func makeIOFileHandle(url: URL) throws -> any MTLIOFileHandle

Creates an input/output file handle instance that represents a file at a URL.

**Required**

func makeIOFileHandle(url: URL, compressionMethod: MTLIOCompressionMethod) throws -> any MTLIOFileHandle

Creates an input/output file handle instance that represents a compressed file at a URL.

**Required**

func makeIOHandle(url: URL, compressionMethod: MTLIOCompressionMethod) throws -> any MTLIOFileHandle

Creates an input/output file handle instance that represents a compressed file at a URL.

**Required**

Deprecated

