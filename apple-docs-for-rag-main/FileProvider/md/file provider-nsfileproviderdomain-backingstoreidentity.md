

- File Provider
- NSFileProviderDomain
-  backingStoreIdentity 

Instance Property

# backingStoreIdentity

A unique identifier for the backing store used by the system.

iOS 16.0+iPadOS 16.0+macOS 12.0+visionOS 1.0+

``` source
var backingStoreIdentity: Data? { get }
```

## Discussion

Changes to this identifier indicate that the system has dropped its backing store and is creating a new one. The system may create a new backing store if the old store becomes corrupted. The file provider extension can also request a new backing store by calling reimportItems(below:completionHandler:).

While rebuilding the backing store, the system invalidates any extension instances associated with the domain. As a result, the system guarantees that the backingStoreIdentity remains stable throughout the lifetime of an NSFileProviderReplicatedExtension instance.

Note

This property is only available on file provider extensions based on the NSFileProviderReplicatedExtension protocol.

## See Also

### Accessing data

var displayName: String

The name of the domain displayed in the user interface.

var identifier: NSFileProviderDomainIdentifier

The domain’s unique identifier.

var isReplicated: Bool

var pathRelativeToDocumentStorage: String

The path of the domain’s subdirectory relative to the file provider’s shared container.

var isHidden: Bool

A Boolean value that determines whether the domain is visible to users.

var userEnabled: Bool

A Boolean value that indicates whether the user has enabled or disabled the domain.

var isDisconnected: Bool

A Boolean value indicating that the domain is present, but disconnected from the file extension.

var supportsSyncingTrash: Bool

var userInfo: [AnyHashable : Any]?

var volumeUUID: UUID?

