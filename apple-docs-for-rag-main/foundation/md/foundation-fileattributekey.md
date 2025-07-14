

- Foundation
-  FileAttributeKey 

Structure

# FileAttributeKey

Keys in dictionaries used to get and set file attributes.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
struct FileAttributeKey
```

## Discussion

These keys are used with the methods listed in the Getting and Setting Attributes topic of FileManager.

## Topics

### Creating a File Attribute Key

init(String)

Creates a file attribute key from a string.

init(rawValue: String)

### Accessing File Attributes

static let appendOnly: FileAttributeKey

The key in a file attribute dictionary whose value indicates whether the file is read-only.

static let busy: FileAttributeKey

The key in a file attribute dictionary whose value indicates whether the file is busy.

static let creationDate: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s creation date.

static let deviceIdentifier: FileAttributeKey

The key in a file attribute dictionary whose value indicates the identifier for the device on which the file resides.

static let extensionHidden: FileAttributeKey

The key in a file attribute dictionary whose value indicates whether the file’s extension is hidden.

static let groupOwnerAccountID: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s group ID.

static let groupOwnerAccountName: FileAttributeKey

The key in a file attribute dictionary whose value indicates the group name of the file’s owner.

static let hfsCreatorCode: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s HFS creator code.

static let hfsTypeCode: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s HFS type code.

static let immutable: FileAttributeKey

The key in a file attribute dictionary whose value indicates whether the file is mutable.

static let modificationDate: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s last modified date.

static let ownerAccountID: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s owner’s account ID.

static let ownerAccountName: FileAttributeKey

The key in a file attribute dictionary whose value indicates the name of the file’s owner.

static let posixPermissions: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s Posix permissions.

static let protectionKey: FileAttributeKey

The key in a file attribute dictionary whose value identifies the protection level for this file.

static let referenceCount: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s reference count.

static let size: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s size in bytes.

static let systemFileNumber: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s filesystem file number.

static let systemFreeNodes: FileAttributeKey

The key in a file system attribute dictionary whose value indicates the number of free nodes in the file system.

static let systemFreeSize: FileAttributeKey

The key in a file system attribute dictionary whose value indicates the amount of free space on the file system.

static let systemNodes: FileAttributeKey

The key in a file system attribute dictionary whose value indicates the number of nodes in the file system.

static let systemNumber: FileAttributeKey

The key in a file system attribute dictionary whose value indicates the filesystem number of the file system.

static let systemSize: FileAttributeKey

The key in a file system attribute dictionary whose value indicates the size of the file system.

static let type: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s type.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Supporting Types

struct DirectoryEnumerationOptions

Options for enumerating the contents of directories.

enum SearchPathDirectory

The location of significant directories.

struct SearchPathDomainMask

Domain constants specifying base locations to use when you search for significant directories.

struct FileAttributeType

Values representing a file’s type attribute.

struct FileProtectionType

Protection level values that can be associated with a file attribute key.

struct URLFileProtection

Protection-level values for a URL resource key.

