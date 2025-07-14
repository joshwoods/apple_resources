

- File Provider
-  NSFileProviderDomain 

Class

# NSFileProviderDomain

A File Provider extension’s domain.

iOS 11.0+iPadOS 11.0+macOS 11.0+visionOS 1.0+

``` source
class NSFileProviderDomain
```

## Overview

You can use domains to partition a file provider’s content. When you use domains, a single file provider can act as if multiple file providers were installed, and users can dynamically switch from one domain to another. You can use domains to represent different accounts or locations.

By default, a File Provider extension has no domain. You can register domains by calling the NSFileProviderManager class’s add(_:completionHandler:) method. A new NSFileProviderExtension instance is created for each domain that you register. The NSFileProviderExtension object’s domain property indicates which domain the file provider belongs to. Any items returned by that file provider also belong to the domain.

## Topics

### Creating domains

init(identifier: NSFileProviderDomainIdentifier, displayName: String, pathRelativeToDocumentStorage: String)

Returns a newly instantiated domain.

init(identifier: NSFileProviderDomainIdentifier, displayName: String)

Creates a new file provider domain with the specified identifier and display name.

struct NSFileProviderDomainIdentifier

A unique identifier for a file provider’s domain.

init(displayName: String, userInfo: [AnyHashable : Any], volumeURL: URL?)

Creates a new file provider domain with the specified URL and display name.

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

var isDisconnected: Bool

A Boolean value indicating that the domain is present, but disconnected from the file extension.

var supportsSyncingTrash: Bool

var userInfo: [AnyHashable : Any]?

var volumeUUID: UUID?

### Syncing Desktop and Documents folders

var replicatedKnownFolders: NSFileProviderKnownFolders

A list of known folders that the domain currently replicates.

var supportedKnownFolders: NSFileProviderKnownFolders

A list of known folders that the domain can replicate.

struct NSFileProviderKnownFolders

Constants that identify known folders.

### Testing

var testingModes: NSFileProviderDomain.TestingModes

A mode that gives the File Provider extension more control over the system’s behavior during testing.

struct TestingModes

Modes that modify the system’s behavior while testing.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

