

- GameKit
- GKMatchDelegate
-  match(\_:shouldReinvitePlayer:) Deprecated

Instance Method

# match(\_:shouldReinvitePlayer:)

Handles when a player disconnects from a two-player match.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func match(
    _ match: GKMatch,
    shouldReinvitePlayer playerID: String
) -> Bool
```

## Parameters 

`match`  

The match that lost the player.

`playerID`  

The identifier for the player whose connection failed.

## Return Value

Your game should return true if it wants GameKit to attempt to reconnect the player, false if it wants to terminate the match.

## Discussion

Occasionally, players may get disconnected from a match. If your game implements this method in the match delegate and the match only contains two players, GameKit calls this method after a player gets disconnected. If your delegate allows GameKit to reconnect to the other player, it reconnects the other player. Your match(_:player:didChange:) method is called when the other player is reconnected.

## See Also

### Deprecated Methods and Properties

func match(GKMatch, player: String, didChange: GKPlayerConnectionState)

Handles when a player connects or disconnects from a match.

Deprecated

func match(GKMatch, didReceive: Data, fromPlayer: String)

Handles when a player receives data in a match.

Deprecated

