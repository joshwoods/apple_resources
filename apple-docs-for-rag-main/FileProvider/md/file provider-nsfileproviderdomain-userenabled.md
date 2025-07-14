

- File Provider
- NSFileProviderDomain
-  userEnabled 

Instance Property

# userEnabled

A Boolean value that indicates whether the user has enabled or disabled the domain.

iOS 16.0+iPadOS 16.0+macOS 11.0+visionOS 1.0+

``` source
var userEnabled: Bool { get }
```

## Discussion

By default, the property is true; however, If the user disables the domain in the System Preferences, the property is false.

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

var isDisconnected: Bool

A Boolean value indicating that the domain is present, but disconnected from the file extension.

var supportsSyncingTrash: Bool

var userInfo: [AnyHashable : Any]?

var volumeUUID: UUID?

