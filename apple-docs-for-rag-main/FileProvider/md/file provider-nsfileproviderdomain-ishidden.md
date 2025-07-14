

- File Provider
- NSFileProviderDomain
-  isHidden 

Instance Property

# isHidden

A Boolean value that determines whether the domain is visible to users.

macOS 11.0+

``` source
var isHidden: Bool { get set }
```

## Discussion

The system stores the files on disk, but it doesn’t display them to the user. For example, you could set this value to false when performing a dry run of a migration.

## See Also

### Accessing data

var displayName: String

The name of the domain displayed in the user interface.

var identifier: NSFileProviderDomainIdentifier

The domain’s unique identifier.

var isReplicated: Bool

var backingStoreIdentity: Data?

A unique identifier for the backing store used by the system.

var pathRelativeToDocumentStorage: String

The path of the domain’s subdirectory relative to the file provider’s shared container.

var userEnabled: Bool

A Boolean value that indicates whether the user has enabled or disabled the domain.

var isDisconnected: Bool

A Boolean value indicating that the domain is present, but disconnected from the file extension.

var supportsSyncingTrash: Bool

var userInfo: [AnyHashable : Any]?

var volumeUUID: UUID?

