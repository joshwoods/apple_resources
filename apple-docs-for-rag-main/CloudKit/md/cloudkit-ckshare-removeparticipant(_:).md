

- CloudKit
- CKShare
-  removeParticipant(\_:) 

Instance Method

# removeParticipant(\_:)

Removes a participant from the share.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
func removeParticipant(_ participant: CKShare.Participant)
```

## Parameters 

`participant`  

The participant to remove from the share.

## Discussion

To modify the list of participants, a share’s publicPermission must be CKShare.ParticipantPermission.none. You can’t mix and match public and private users in the same share. You can only add certain participant types with this API. See CKShare.Participant for more information.

## See Also

### Configuring the Share

var publicPermission: CKShare.ParticipantPermission

The permission for anyone with access to the share’s URL.

func addParticipant(CKShare.Participant)

Adds a participant to the share.

class Participant

An object that describes a user’s participation in a share.

