

- CloudKit
- CKShare
- CKShare.Participant
-  permission 

Instance Property

# permission

The participant’s permission level for the share.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var permission: CKShare.ParticipantPermission { get set }
```

## Discussion

This property controls the permissions that the participant has for the share. For a list of possible values, see CKShare.ParticipantPermission.

## See Also

### Managing the Participant’s Capabilites

typealias Permission

A type that represents the permissions for a participant.

enum ParticipantPermission

Constants that represent the permissions to grant to a share participant.

var role: CKShare.ParticipantRole

The participant’s role for the share.

typealias Role

A type that represents the role for a participant.

enum ParticipantRole

Constants that represent the role of a share’s participant.

