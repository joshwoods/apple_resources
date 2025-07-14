

- CloudKit
- CKAllowedSharingOptions
-  allowedParticipantPermissionOptions 

Instance Property

# allowedParticipantPermissionOptions

The permission option the system uses to control whether a user can grant read-only or write access.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
var allowedParticipantPermissionOptions: CKSharingParticipantPermissionOption { get set }
```

## See Also

### Configuring the options

var allowedParticipantAccessOptions: CKSharingParticipantAccessOption

The permission option the system uses to control whether a user can share publicly or privately.

struct CKSharingParticipantAccessOption

An object that controls participant access options.

struct CKSharingParticipantPermissionOption

An object that controls participant permission options.

