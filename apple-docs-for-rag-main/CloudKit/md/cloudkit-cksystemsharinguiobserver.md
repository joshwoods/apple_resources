

- CloudKit
-  CKSystemSharingUIObserver 

Class

# CKSystemSharingUIObserver

An object the system uses to monitor changes in sharing.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class CKSystemSharingUIObserver
```

## Overview

Initialize a `CKSystemSharingUIObserver` instance with your CKContainer when preparing to share an item using the share sheet. Use your implementation to update the local state of a shared item when your app receives a CKShare, or to delete a locally cached share when the system notifies your app about a share deletion.

The system only propagates changes on the local device using `CKSystemSharingUIObserver`. The system doesn’t notify your app about any remote changes on the server. For more information about how to keep your local cache in sync with remote changes, see Remote Records.

## Topics

### Creating a sharing observer

init(container: CKContainer)

Creates and initializes an observer using the provided container.

### Accessing sharing blocks

var systemSharingUIDidSaveShareBlock: ((CKRecord.ID, Result&lt;CKShare, any Error>) -> Void)?

A callback block the system invokes after the success or failure of a system sharing UI save.

var systemSharingUIDidStopSharingBlock: ((CKRecord.ID, Result&lt;Void, any Error>) -> Void)?

A callback block the system invokes after the success or failure of a system sharing UI delete.

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
- Sendable

## See Also

### Collaboration

Sharing CloudKit Data with Other iCloud Users

Create and share private CloudKit data with other users by implementing the sharing UI.

Sharing Core Data objects between iCloud users

Use Core Data and CloudKit to synchronize data between devices of an iCloud user and share data between different iCloud users.

class CKShare

A specialized record type that manages a collection of shared records.

struct CKShareTransferRepresentation

A transfer representation the system uses to share an item.

class CKAllowedSharingOptions

An object that controls participant access and permission options.

@MainActor class UICloudSharingController

A view controller that presents standard screens for adding and removing people from a CloudKit share record.

CKSharingSupported

A Boolean value that indicates your app supports CloudKit Sharing.

