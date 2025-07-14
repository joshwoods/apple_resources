

- GameKit
- GKMatchmaker
-  cancelInvite(toPlayer:) Deprecated

Instance Method

# cancelInvite(toPlayer:)

Cancels a pending invitation to another player.

iOS 6.0–8.0DeprecatediPadOS 6.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func cancelInvite(toPlayer playerID: String)
```

Deprecated

Use the cancelPendingInvite(to:) method instead.

## Parameters 

`playerID`  

The player identifier for a player that GameKit previously invited to the match.

## See Also

### Deprecated Methods

func findPlayers(forHostedMatchRequest: GKMatchRequest, withCompletionHandler: (([String]?, (any Error)?) -> Void)?)

Initiates a request to find players for a hosted match.

Deprecated

func startBrowsingForNearbyPlayers(reachableHandler: ((String, Bool) -> Void)?)

Enables the matchmaking process to find nearby players through Bluetooth or WiFi, but only on the same subnet.

Deprecated

