

- Foundation
-  URLFileResourceType 

Structure

# URLFileResourceType

Possible values for the type of file resource.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct URLFileResourceType
```

## Topics

### Creating a File Resource Type Instance

init(rawValue: String)

### Constants

static let namedPipe: URLFileResourceType

The resource is a named pipe.

static let characterSpecial: URLFileResourceType

The resource is a character special file.

static let directory: URLFileResourceType

The resource is a directory.

static let blockSpecial: URLFileResourceType

The resource is a block special file.

static let regular: URLFileResourceType

The resource is a regular file.

static let symbolicLink: URLFileResourceType

The resource is a symbolic link.

static let socket: URLFileResourceType

The resource is a socket.

static let unknown: URLFileResourceType

The resource’s type is unknown.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### File keys

static let fileAllocatedSizeKey: URLResourceKey

The key for the total allocated size on-disk for the file.

static let fileProtectionKey: URLResourceKey

The key for the protection level of the file.

struct URLFileProtection

Protection-level values for a URL resource key.

static let fileContentIdentifierKey: URLResourceKey

The key for a value that APFS assigns to identify a file’s content data stream.

static let fileResourceIdentifierKey: URLResourceKey

The key for the resource’s unique identifier.

static let fileResourceTypeKey: URLResourceKey

The key for the resource’s object type.

static let fileSecurityKey: URLResourceKey

The key for the resource’s security information.

static let fileSizeKey: URLResourceKey

The key for the file’s size, in bytes.

static let isAliasFileKey: URLResourceKey

The key for determining whether the file is an alias.

static let isPackageKey: URLResourceKey

The key for determining whether the resource is a file package.

static let isRegularFileKey: URLResourceKey

The key for determining whether the resource is a regular file rather than a directory or a symbolic link.

static let isPurgeableKey: URLResourceKey

The key for a Boolean value that indicates whether the file system can delete a file when the system needs to free space.

static let isSparseKey: URLResourceKey

The key for a Boolean value that indicates whether the file has sparse regions.

static let mayHaveExtendedAttributesKey: URLResourceKey

The key for a Boolean value that indicates whether the file has extended attributes.

static let mayShareFileContentKey: URLResourceKey

The key for a Boolean value that indicates whether cloned files and their original files may share data blocks.

