

- CloudKit
-  CKAllowedSharingOptions 

Class

# CKAllowedSharingOptions

An object that controls participant access and permission options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class CKAllowedSharingOptions
```

## Overview

Register an instance of this class with an NSItemProvider or when preparing a CKShareTransferRepresentation.ExportedShare before your app invokes the share sheet. The share sheet uses the registered `CKAllowedSharingOptions` object to let the user choose between the allowed options when sharing.

## Topics

### Creating sharing options

init(allowedParticipantPermissionOptions: CKSharingParticipantPermissionOption, allowedParticipantAccessOptions: CKSharingParticipantAccessOption)

Creates and initializes an allowed sharing options object.

### Using the standard options

class var standard: CKAllowedSharingOptions

An object set to the most permissive sharing options.

### Configuring the options

var allowedParticipantAccessOptions: CKSharingParticipantAccessOption

The permission option the system uses to control whether a user can share publicly or privately.

var allowedParticipantPermissionOptions: CKSharingParticipantPermissionOption

The permission option the system uses to control whether a user can grant read-only or write access.

struct CKSharingParticipantAccessOption

An object that controls participant access options.

struct CKSharingParticipantPermissionOption

An object that controls participant permission options.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding
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

class CKSystemSharingUIObserver

An object the system uses to monitor changes in sharing.

@MainActor class UICloudSharingController

A view controller that presents standard screens for adding and removing people from a CloudKit share record.

CKSharingSupported

A Boolean value that indicates your app supports CloudKit Sharing.

