

- GameKit
- GKMatchmaker
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

## Topics

### Deprecated Properties

var inviteHandler: ((GKInvite, [Any]?) -> Void)?

A block that GameKit calls when an invitation to join a match is accepted by the local player.

Deprecated

### Deprecated Methods

func cancelInvite(toPlayer: String)

Cancels a pending invitation to another player.

Deprecated

func findPlayers(forHostedMatchRequest: GKMatchRequest, withCompletionHandler: (([String]?, (any Error)?) -> Void)?)

Initiates a request to find players for a hosted match.

Deprecated

func startBrowsingForNearbyPlayers(reachableHandler: ((String, Bool) -> Void)?)

Enables the matchmaking process to find nearby players through Bluetooth or WiFi, but only on the same subnet.

Deprecated

