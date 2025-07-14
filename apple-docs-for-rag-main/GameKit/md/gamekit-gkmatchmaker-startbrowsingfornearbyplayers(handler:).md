

- GameKit
- GKMatchmaker
-  startBrowsingForNearbyPlayers(handler:) 

Instance Method

# startBrowsingForNearbyPlayers(handler:)

Finds nearby players through Bluetooth or WiFi on the same subnet.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+

``` source
func startBrowsingForNearbyPlayers(handler reachableHandler: ((GKPlayer, Bool) -> Void)? = nil)
```

## Parameters 

`reachableHandler`  

The block that GameKit calls when it completes the request.

This block receives the following parameters:

`player`  
The player whose reachability status changes.

`reachable`  
true if a new nearby player appears. false if a previously discovered player disappears.

## Discussion

Use the `reachableHandler` implementation to update your interface with information about nearby players. If the local player wants to invite a nearby player, call the findMatch(for:withCompletionHandler:) method to create a match or the addPlayers(to:matchRequest:completionHandler:) method to update an existing match. When you are done finding nearby players, call the stopBrowsingForNearbyPlayers() method.

Note

Before your game is released and during development, GameKit invokes the handler for all nearby players of all Game Center games.

## See Also

### Looking for nearby players

func stopBrowsingForNearbyPlayers()

Stops finding nearby players.

