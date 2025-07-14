

- GameKit
- GKPlayer
-  loadPlayers(forIdentifiers:withCompletionHandler:) Deprecated

Type Method

# loadPlayers(forIdentifiers:withCompletionHandler:)

Loads information about a list of players from Game Center.

iOS 4.1–14.5DeprecatediPadOS 4.1–14.5DeprecatedMac Catalyst 13.1–14.5DeprecatedmacOS 10.8–11.3DeprecatedtvOS 9.0–14.5DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.4Deprecated

``` source
class func loadPlayers(
    forIdentifiers identifiers: [String],
    withCompletionHandler completionHandler: (([GKPlayer]?, (any Error)?) -> Void)? = nil
)
```

Deprecated

Use loadFriends(identifiedBy:completionHandler:) instead.

## Parameters 

`identifiers`  

The identifiers for the players to load.

`completionHandler`  

The block that GameKit calls when it completes the request.

The block receives the following parameters:

*players*  
The players that GameKit successfully loads. If an error occurs, this array may contain just the player data that GameKit is able to load.

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

