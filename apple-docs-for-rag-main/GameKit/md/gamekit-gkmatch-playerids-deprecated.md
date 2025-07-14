

- GameKit
- GKMatch
-  playerIDs Deprecated

Instance Property

# playerIDs

The player identifiers for remote players in the match.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var playerIDs: [String]? { get }
```

Deprecated

Use the players property instead.

## Discussion

The `playerIDs` property initially includes the player identifiers for any remote players already connected to the match; the array may initially be empty. As each new player connects to the match, GameKit adds the player’s identifier to the array. GameKit doesn’t include the local player’s identifier in this array.

## See Also

### Related Documentation

var expectedPlayerCount: Int

The remaining number of players invited but not yet connected to the match.

### Deprecated Methods and Properties

func chooseBestHostPlayer(completionHandler: (String?) -> Void)

Determines the best player in the game to act as the server for a client-server match.

Deprecated

func send(Data, toPlayers: [String], with: GKMatch.SendDataMode) throws

Transmits data to a list of connected players.

Deprecated

