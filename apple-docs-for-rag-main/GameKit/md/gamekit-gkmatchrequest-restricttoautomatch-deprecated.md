

- GameKit
- GKMatchRequest
-  restrictToAutomatch Deprecated

Instance Property

# restrictToAutomatch

A Boolean value that determines whether a game uses automatch to find players or the local player invites players.

iOS 13.0–14.0DeprecatediPadOS 13.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.15–11.0DeprecatedtvOS 13.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 6.0–7.0Deprecated

``` source
var restrictToAutomatch: Bool { get set }
```

Deprecated

Use the matchmakingMode property instead.

## Discussion

Use this property to match the local player only with players who are also actively looking for a match. If true, the local player can’t invite contacts, friends, or nearby players. The default value is false.

## See Also

### Deprecated methods and properties

var inviteeResponseHandler: ((String, GKInviteeResponse) -> Void)?

Handles when a player responds to an invitation.

Deprecated

typealias GKInviteeResponse

Possible responses from an invitation to a remote player.

Deprecated

var playersToInvite: [String]?

A list of player identifiers for players to invite to the match.

Deprecated

