

- GameKit
- GKMatchmaker
-  startBrowsingForNearbyPlayers(reachableHandler:) Deprecated

Instance Method

# startBrowsingForNearbyPlayers(reachableHandler:)

Enables the matchmaking process to find nearby players through Bluetooth or WiFi, but only on the same subnet.

iOS 6.0–8.0DeprecatediPadOS 6.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func startBrowsingForNearbyPlayers(reachableHandler: ((String, Bool) -> Void)? = nil)
```

Deprecated

Use the startBrowsingForNearbyPlayers(handler:) method instead.

## Parameters 

`reachableHandler`  

A block to call when the reachability for a player changes. The block takes the following parameters:

*playerID*  
The player identifier for the player whose reachability status has changed.

*reachable*  
true if GameKit discovers a new player locally, false if a previously discovered player disappears.

## Discussion

Use this method only when you are implementing programmatic matchmaking. After enabling browsing for nearby players, use the responses to populate your user interface with information about nearby players. If a player wants to invite a player to a game, add that player’s player identifier to a match request and call either the findMatch(for:withCompletionHandler:) to create a match or addPlayers(to:matchRequest:completionHandler:) method to update a match.

## See Also

### Deprecated Methods

func cancelInvite(toPlayer: String)

Cancels a pending invitation to another player.

Deprecated

func findPlayers(forHostedMatchRequest: GKMatchRequest, withCompletionHandler: (([String]?, (any Error)?) -> Void)?)

Initiates a request to find players for a hosted match.

Deprecated

