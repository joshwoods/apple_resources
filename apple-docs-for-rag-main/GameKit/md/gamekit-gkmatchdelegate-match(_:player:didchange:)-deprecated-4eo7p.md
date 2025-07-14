

- GameKit
- GKMatchDelegate
-  match(\_:player:didChange:) Deprecated

Instance Method

# match(\_:player:didChange:)

Handles when a player connects or disconnects from a match.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedvisionOS 1.0–1.0Deprecated

``` source
optional func match(
    _ match: GKMatch,
    player playerID: String,
    didChange state: GKPlayerConnectionState
)
```

## Parameters 

`match`  

The match that the player is connected to.

`playerID`  

The identifier for the player whose state changed.

`state`  

The state the player moved to.

## Discussion

Implement this method to be notified when players connect to or disconnect from the match.

## See Also

### Deprecated Methods and Properties

func match(GKMatch, didReceive: Data, fromPlayer: String)

Handles when a player receives data in a match.

Deprecated

func match(GKMatch, shouldReinvitePlayer: String) -> Bool

Handles when a player disconnects from a two-player match.

Deprecated

