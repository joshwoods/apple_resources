

- File Provider
- NSFileProviderDomain
-  isDisconnected 

Instance Property

# isDisconnected

A Boolean value indicating that the domain is present, but disconnected from the file extension.

macOS 11.0+

``` source
var isDisconnected: Bool { get }
```

## Discussion

Users can continue to browse the content from a disconnected domain; however, the File Provider extension no longer sends or receives updates about modifications to the files.

To change the disconnected state, create a new NSFileProviderDomain using the same identifier, and pass it to add(_:completionHandler:).

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

var isHidden: Bool

A Boolean value that determines whether the domain is visible to users.

var userEnabled: Bool

A Boolean value that indicates whether the user has enabled or disabled the domain.

var supportsSyncingTrash: Bool

var userInfo: [AnyHashable : Any]?

var volumeUUID: UUID?

