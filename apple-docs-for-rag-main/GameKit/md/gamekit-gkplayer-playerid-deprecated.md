

- GameKit
- GKPlayer
-  playerID Deprecated

Instance Property

# playerID

A unique identifier for a player of the game.

iOS 4.1–13.0DeprecatediPadOS 4.1–13.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.15DeprecatedtvOS 9.0–13.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–6.0Deprecated

``` source
var playerID: String { get }
```

Deprecated

Use gamePlayerID or teamPlayerID instead.

## Mentioned in 

Protecting the player’s privacy using scoped identifiers

## Discussion

Never display the player identifier to the player. Use it only to identify a player in your code.

## See Also

### Identifying the player

var gamePlayerID: String

A unique identifier for a player of the game.

var teamPlayerID: String

A unique identifier for a player of all the games that you distribute using your developer account.

func scopedIDsArePersistent() -> Bool

Returns a Boolean value depending on whether the player identifiers are persistent across game instances or unique to the game instance.

let GKPlayerIDNoLongerAvailable: String

A constant for a player ID that’s no longer available.

