

- GameKit
- GKMatchRequest
-  playersToInvite Deprecated

Instance Property

# playersToInvite

A list of player identifiers for players to invite to the match.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var playersToInvite: [String]? { get set }
```

Deprecated

Use the recipients property instead.

## Discussion

The property holds an array of NSString objects, each of which is an identifier for a player on Game Center. If the value of the property is non-`nil`, when you use the request to create a match, Game Center invites those players to the match. No automatching is done and the GKMatchRequest `maxPlayers` and `minPlayers` properties are ignored. If `nil` (the default), no players are invited. The exact behavior for matchmaking depends on the kind of match being created and the class used to create the match.

## See Also

### Deprecated methods and properties

var inviteeResponseHandler: ((String, GKInviteeResponse) -> Void)?

Handles when a player responds to an invitation.

Deprecated

typealias GKInviteeResponse

Possible responses from an invitation to a remote player.

Deprecated

var restrictToAutomatch: Bool

A Boolean value that determines whether a game uses automatch to find players or the local player invites players.

Deprecated

