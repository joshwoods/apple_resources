

- GameKit
- GKMatchRequest
-  inviteeResponseHandler Deprecated

Instance Property

# inviteeResponseHandler

Handles when a player responds to an invitation.

iOS 6.0–8.0DeprecatediPadOS 6.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var inviteeResponseHandler: ((String, GKInviteeResponse) -> Void)? { get set }
```

Deprecated

Use the recipientResponseHandler property instead.

## Discussion

The block takes the following parameters:

*playerID*  
The identifier for the player.

*GKInviteeResponse*  
The nature of the response. See GKInviteeResponse.

An invitee response handler is called whenever you programmatically invite specific players to join a match. It is called once for each player invited to the match. Typically, your game uses the responses to update the custom user interface. For example, you want the player to be able to perform any of the following tasks:

- Start the match.

- Invite an additional set of specific players.

- Use matchmaking to fill the remaining match slots.

## See Also

### Deprecated methods and properties

typealias GKInviteeResponse

Possible responses from an invitation to a remote player.

Deprecated

var playersToInvite: [String]?

A list of player identifiers for players to invite to the match.

Deprecated

var restrictToAutomatch: Bool

A Boolean value that determines whether a game uses automatch to find players or the local player invites players.

Deprecated

