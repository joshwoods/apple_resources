

- CloudKit
- CKShare
-  owner 

Instance Property

# owner

The participant that represents the share’s owner.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
@NSCopying
var owner: CKShare.Participant { get }
```

## See Also

### Accessing the Share’s Attributes

var currentUserParticipant: CKShare.Participant?

The participant that represents the current user.

var participants: [CKShare.Participant]

An array that contains the share’s participants.

var url: URL?

The URL for inviting participants to the share.

