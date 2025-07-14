

- GameKit
- GKPlayer
-  teamPlayerID 

Instance Property

# teamPlayerID

A unique identifier for a player of all the games that you distribute using your developer account.

iOS 12.4+iPadOS 12.4+Mac Catalyst 13.1+macOS 10.14.6+tvOS 12.4+visionOS 1.0+

``` source
var teamPlayerID: String { get }
```

## Mentioned in 

Protecting the player’s privacy using scoped identifiers

## Discussion

This identifier is unique to this game instance if the scopedIDsArePersistent() method returns false. Otherwise, this identifier is the same across all game instances of your games that use the same developer Team ID. An instance is the time between when the game launches and when the game terminates. For more information about the Team ID, see Locate your Team ID.

For the local player (a GKLocalPlayer object), this identifier is the same across all local player instances of your games. If the player is friends with the local player, this identifier is the same across all local player and friend game instances. To determine whether the player is a friend, use the loadFriends(_:) method.

To protect the player’s privacy, use the gamePlayerID property instead of the teamPlayerID property. If you need to use the teamPlayerID for tracking players across multiple games, also store the gamePlayerID property. For more information, see Protecting the player’s privacy using scoped identifiers.

If you transfer your game to another developer, the teamPlayerID property isn’t the same for the new developer. For more information, see Overview of app transfer.

## See Also

### Identifying the player

var gamePlayerID: String

A unique identifier for a player of the game.

func scopedIDsArePersistent() -> Bool

Returns a Boolean value depending on whether the player identifiers are persistent across game instances or unique to the game instance.

let GKPlayerIDNoLongerAvailable: String

A constant for a player ID that’s no longer available.

var playerID: String

A unique identifier for a player of the game.

Deprecated

