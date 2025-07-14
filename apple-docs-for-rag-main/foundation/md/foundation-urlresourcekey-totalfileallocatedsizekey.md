

- Foundation
- URLResourceKey
-  totalFileAllocatedSizeKey 

Type Property

# totalFileAllocatedSizeKey

The key for the total allocated size of the file, in bytes.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let totalFileAllocatedSizeKey: URLResourceKey
```

## Discussion

The system returns the read-only value as an NSNumber object. The values includes the size of any file metadata.

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

struct URLFileResourceType

Possible values for the type of file resource.

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

