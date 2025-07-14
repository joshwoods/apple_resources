

- CloudKit
- CKShare
-  addParticipant(\_:) 

Instance Method

# addParticipant(\_:)

Adds a participant to the share.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func addParticipant(_ participant: CKShare.Participant)
```

## Parameters 

`participant`  

The participant to add to the share.

## Discussion

If a participant with a matching userIdentity already exists in the share, the system updates the existing participant’s properties and doesn’t add a new participant.

To modify the list of participants, a share’s publicPermission must be CKShare.ParticipantPermission.none. You can’t mix and match public and private users in the same share. You can only add certain participant types with this API. See CKShare.Participant for more information.

## See Also

### Configuring the Share

var publicPermission: CKShare.ParticipantPermission

The permission for anyone with access to the share’s URL.

func removeParticipant(CKShare.Participant)

Removes a participant from the share.

class Participant

An object that describes a user’s participation in a share.

