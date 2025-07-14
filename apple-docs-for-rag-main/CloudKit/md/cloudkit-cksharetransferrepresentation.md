

- CloudKit
-  CKShareTransferRepresentation 

Structure

# CKShareTransferRepresentation

A transfer representation the system uses to share an item.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS

``` source
struct CKShareTransferRepresentation where Item : Transferable
```

## Topics

### Creating a transfer representation

init(exporter: (Item) throws -> CKShareTransferRepresentation&lt;Item>.ExportedShare)

Creates and initializes a transfer representation.

### Accessing transfer representation attributes

struct ExportedShare

An intermediate structure that returns an existing share or prepares a new one if it doesn’t exist.

## Relationships

### Conforms To

- Sendable
- TransferRepresentation

## See Also

### Collaboration

Sharing CloudKit Data with Other iCloud Users

Create and share private CloudKit data with other users by implementing the sharing UI.

Sharing Core Data objects between iCloud users

Use Core Data and CloudKit to synchronize data between devices of an iCloud user and share data between different iCloud users.

class CKShare

A specialized record type that manages a collection of shared records.

class CKAllowedSharingOptions

An object that controls participant access and permission options.

class CKSystemSharingUIObserver

An object the system uses to monitor changes in sharing.

@MainActor class UICloudSharingController

A view controller that presents standard screens for adding and removing people from a CloudKit share record.

CKSharingSupported

A Boolean value that indicates your app supports CloudKit Sharing.

