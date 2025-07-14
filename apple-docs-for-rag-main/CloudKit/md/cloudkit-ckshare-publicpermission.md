

- CloudKit
- CKShare
-  publicPermission 

Instance Property

# publicPermission

The permission for anyone with access to the share’s URL.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var publicPermission: CKShare.ParticipantPermission { get set }
```

## Discussion

Setting this property’s value to be more permissive than CKShare.ParticipantPermission.none allows any user with the share’s URL to join. CloudKit removes all public participants when you save the share if you set the property’s value to CKShare.ParticipantPermission.none.

The default value is CKShare.ParticipantPermission.none

## See Also

### Configuring the Share

func addParticipant(CKShare.Participant)

Adds a participant to the share.

func removeParticipant(CKShare.Participant)

Removes a participant from the share.

class Participant

An object that describes a user’s participation in a share.

