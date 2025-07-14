

- CloudKit
-  CKSharingParticipantPermissionOption 

Structure

# CKSharingParticipantPermissionOption

An object that controls participant permission options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct CKSharingParticipantPermissionOption
```

## Topics

### Creating an access option

init(rawValue: UInt)

Creates and initializes a participant permission option object.

### Configuring the options

static var any: CKSharingParticipantPermissionOption

The permission option the system uses to control whether a user can grant read-only or write access.

static var readOnly: CKSharingParticipantPermissionOption

The permission option the system uses to control whether a user can grant read-only access.

static var readWrite: CKSharingParticipantPermissionOption

The permission option the system uses to control whether a user can grant write access.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Configuring the options

var allowedParticipantAccessOptions: CKSharingParticipantAccessOption

The permission option the system uses to control whether a user can share publicly or privately.

var allowedParticipantPermissionOptions: CKSharingParticipantPermissionOption

The permission option the system uses to control whether a user can grant read-only or write access.

struct CKSharingParticipantAccessOption

An object that controls participant access options.

