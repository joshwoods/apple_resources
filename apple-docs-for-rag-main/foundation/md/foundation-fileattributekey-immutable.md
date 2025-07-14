

- Foundation
- FileAttributeKey
-  immutable 

Type Property

# immutable

The key in a file attribute dictionary whose value indicates whether the file is mutable.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let immutable: FileAttributeKey
```

## Discussion

The corresponding value is an NSNumber object containing a Boolean value.

## See Also

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

