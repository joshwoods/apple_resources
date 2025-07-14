

- CloudKit
-  CKSharingParticipantAccessOption 

Structure

# CKSharingParticipantAccessOption

An object that controls participant access options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
struct CKSharingParticipantAccessOption
```

## Topics

### Creating an access option

init(rawValue: UInt)

Creates and initializes a participant access option object.

### Configuring the options

static var any: CKSharingParticipantAccessOption

The permission option the system uses to control whether a user can share publicly or privately.

static var anyoneWithLink: CKSharingParticipantAccessOption

The permission option the system uses to control whether a user can share publicly.

static var specifiedRecipientsOnly: CKSharingParticipantAccessOption

The permission option the system uses to control whether a user can share privately.

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

struct CKSharingParticipantPermissionOption

An object that controls participant permission options.

