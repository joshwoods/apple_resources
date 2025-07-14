

- GameKit
-  GKInviteeResponse Deprecated

Type Alias

# GKInviteeResponse

Possible responses from an invitation to a remote player.

iOS 6.0–17.0DeprecatediPadOS 6.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.8–14.0DeprecatedtvOS 9.0–17.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
typealias GKInviteeResponse = GKInviteRecipientResponse
```

## Topics

### Responses

static var inviteeResponseAccepted: GKInviteRecipientResponse

The player accepted the invitation.

static var inviteeResponseDeclined: GKInviteRecipientResponse

The player rejected the invitation.

static var inviteeResponseFailed: GKInviteRecipientResponse

The invitation was unable to be delivered.

static var inviteeResponseIncompatible: GKInviteRecipientResponse

The invitee isn’t running a compatible version of your game.

static var inviteeResponseUnableToConnect: GKInviteRecipientResponse

The invitee couldn’t be contacted.

static var inviteeResponseNoAnswer: GKInviteRecipientResponse

The invitation timed out without an answer.

## See Also

### Deprecated methods and properties

var inviteeResponseHandler: ((String, GKInviteeResponse) -> Void)?

Handles when a player responds to an invitation.

Deprecated

var playersToInvite: [String]?

A list of player identifiers for players to invite to the match.

Deprecated

var restrictToAutomatch: Bool

A Boolean value that determines whether a game uses automatch to find players or the local player invites players.

Deprecated

