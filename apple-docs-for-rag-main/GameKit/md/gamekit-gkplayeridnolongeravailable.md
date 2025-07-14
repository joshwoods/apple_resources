

- GameKit
-  GKPlayerIDNoLongerAvailable 

Global Variable

# GKPlayerIDNoLongerAvailable

A constant for a player ID that’s no longer available.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
let GKPlayerIDNoLongerAvailable: String
```

## Discussion

Deprecated methods that previously returned the player ID return this constant.

## See Also

### Identifying the player

var gamePlayerID: String

A unique identifier for a player of the game.

var teamPlayerID: String

A unique identifier for a player of all the games that you distribute using your developer account.

func scopedIDsArePersistent() -> Bool

Returns a Boolean value depending on whether the player identifiers are persistent across game instances or unique to the game instance.

var playerID: String

A unique identifier for a player of the game.

Deprecated

