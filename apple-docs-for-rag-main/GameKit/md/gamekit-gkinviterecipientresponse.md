

- GameKit
-  GKInviteRecipientResponse 

Enumeration

# GKInviteRecipientResponse

A player’s response to an invitation to join a match.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
enum GKInviteRecipientResponse
```

## Topics

### Responses

case accepted

A response when the player accepts the invitation.

case declined

A response when the player rejects the invitation.

case failed

A response when the system fails to deliver the invitation to the player.

case incompatible

A response when the player isn’t running a compatible version of the game.

case unableToConnect

A response when the system can’t contact the player.

case noAnswer

A response when the invitation times out because the player doesn’t answer it.

### Deprecated Properties

static var inviteeResponseAccepted: GKInviteRecipientResponse

The player accepted the invitation.

Deprecated

static var inviteeResponseDeclined: GKInviteRecipientResponse

The player rejected the invitation.

Deprecated

static var inviteeResponseFailed: GKInviteRecipientResponse

The invitation was unable to be delivered.

Deprecated

static var inviteeResponseIncompatible: GKInviteRecipientResponse

The invitee isn’t running a compatible version of your game.

Deprecated

static var inviteeResponseNoAnswer: GKInviteRecipientResponse

The invitation timed out without an answer.

Deprecated

static var inviteeResponseUnableToConnect: GKInviteRecipientResponse

The invitee couldn’t be contacted.

Deprecated

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inviting players

var inviteMessage: String?

The message sent to other players when the local player invites them to join a match.

var recipients: [GKPlayer]?

The players to invite to the match.

var recipientResponseHandler: ((GKPlayer, GKInviteRecipientResponse) -> Void)?

A method that handles when a player responds to an invitation to join a match.

