

- CloudKit
- CKAllowedSharingOptions
-  standard 

Type Property

# standard

An object set to the most permissive sharing options.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+visionOS 1.0+

``` source
class var standard: CKAllowedSharingOptions { get }
```

## Discussion

The `standardOptions` has allowedParticipantPermissionOptions set to `CKSharingParticipantPermissionOptionAny` and allowedParticipantAccessOptions set to `CKSharingParticipantAccessOptionAny`.

