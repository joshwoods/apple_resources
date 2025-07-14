

- GameKit
- GKMatchmaker
-  findPlayers(forHostedMatchRequest:withCompletionHandler:) Deprecated

Instance Method

# findPlayers(forHostedMatchRequest:withCompletionHandler:)

Initiates a request to find players for a hosted match.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
func findPlayers(
    forHostedMatchRequest request: GKMatchRequest,
    withCompletionHandler completionHandler: (([String]?, (any Error)?) -> Void)? = nil
)
```

**Mac Catalyst, visionOS**

``` source
func findPlayers(forHostedMatchRequest request: GKMatchRequest) async throws -> [String]
```

Deprecated

Use the findPlayers(forHostedRequest:withCompletionHandler:) method instead.

## Parameters 

`request`  

The configuration for the desired match.

`completionHandler`  

A block to call when GameKit creates the match. This block receives the following parameters:

*playerIDs*  
If matchmaking was successful, this parameter contains an array of `NSString` objects containing the players to connect into the match. Otherwise, this parameter is `nil`.

*error*  
If matchmaking was successful, this parameter contains `nil`. Otherwise, this parameter holds an error object that describes the error that occurred.

## Discussion

When GameKit calls this completion handler, your game needs to connect those players to your own server.

On iOS 6, if the match request’s playersToInvite property is non-`NIL`, Game Center only sends invitations out to the players listed in the property. If the playersToInvite property is `NIL`, Game Center then searches for any waiting players that match the request. Prior to iOS 6, GameKit ignores the match request’s playersToInvite property and this method only searches for available players.

## See Also

### Related Documentation

func cancel()

Cancels a matchmaking request.

### Deprecated Methods

func cancelInvite(toPlayer: String)

Cancels a pending invitation to another player.

Deprecated

func startBrowsingForNearbyPlayers(reachableHandler: ((String, Bool) -> Void)?)

Enables the matchmaking process to find nearby players through Bluetooth or WiFi, but only on the same subnet.

Deprecated

