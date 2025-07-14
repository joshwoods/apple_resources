

- Metal
- MTLDevice
-  makeBinaryArchive(descriptor:) 

Instance Method

# makeBinaryArchive(descriptor:)

Creates a Metal binary archive instance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func makeBinaryArchive(descriptor: MTLBinaryArchiveDescriptor) throws -> any MTLBinaryArchive
```

**Required**

## Parameters 

`descriptor`  

An MTLBinaryArchiveDescriptor instance.

## Mentioned in 

Compiling Binary Archives from a Custom Configuration Script

Creating Binary Archives from Device-Built Pipeline State Objects

## See Also

### Creating Binary Shader Archives

class MTLBinaryArchiveDescriptor

A description of a binary shader archive that you want to create.

enum Code

Error codes when creating binary archives of compiled shader code.

let MTLBinaryArchiveDomain: String

The domain for Metal binary archive errors.

