

- Foundation
- URLResourceKey
-  fileIdentifierKey 

Type Property

# fileIdentifierKey

The key for the file system’s internal inode identifier for the item.

iOS 16.4+iPadOS 16.4+Mac Catalyst 16.4+macOS 13.3+tvOS 16.4+visionOS 1.0+watchOS 9.4+

``` source
static let fileIdentifierKey: URLResourceKey
```

## Discussion

The value associated with this key isn’t stable for all file systems or across all mounts. Use this value sparingly and don’t persist it. You can use it, for example, to match URLs from the URL enumerator with paths from `FSEvents`.

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

