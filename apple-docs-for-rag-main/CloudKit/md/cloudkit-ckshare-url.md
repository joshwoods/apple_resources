

- CloudKit
- CKShare
-  url 

Instance Property

# url

The URL for inviting participants to the share.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
var url: URL? { get }
```

## Discussion

This property is only available after saving a share record to the server. This URL is stable and persists across shares and reshares of the same root record.

## See Also

### Accessing the Share’s Attributes

var owner: CKShare.Participant

The participant that represents the share’s owner.

var currentUserParticipant: CKShare.Participant?

The participant that represents the current user.

var participants: [CKShare.Participant]

An array that contains the share’s participants.

