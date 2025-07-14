

- Foundation
- FileAttributeKey
-  protectionKey 

Type Property

# protectionKey

The key in a file attribute dictionary whose value identifies the protection level for this file.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static let protectionKey: FileAttributeKey
```

## Discussion

The corresponding value is an NSString value. For a list of possible values, see `File Protection Values`.

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

static let referenceCount: FileAttributeKey

The key in a file attribute dictionary whose value indicates the file’s reference count.

