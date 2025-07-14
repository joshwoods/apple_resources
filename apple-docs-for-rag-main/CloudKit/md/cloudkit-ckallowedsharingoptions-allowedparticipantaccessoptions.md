

- CloudKit
- CKAllowedSharingOptions
-  allowedParticipantAccessOptions 

Instance Property

# allowedParticipantAccessOptions

The permission option the system uses to control whether a user can share publicly or privately.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var allowedParticipantAccessOptions: CKSharingParticipantAccessOption { get set }
```

## See Also

### Configuring the options

var allowedParticipantPermissionOptions: CKSharingParticipantPermissionOption

The permission option the system uses to control whether a user can grant read-only or write access.

struct CKSharingParticipantAccessOption

An object that controls participant access options.

struct CKSharingParticipantPermissionOption

An object that controls participant permission options.

