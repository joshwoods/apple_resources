

- GameKit
- GKPlayer
-  scopedIDsArePersistent() 

Instance Method

# scopedIDsArePersistent()

Returns a Boolean value depending on whether the player identifiers are persistent across game instances or unique to the game instance.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+tvOS 13.0+visionOS 1.0+

``` source
func scopedIDsArePersistent() -> Bool
```

## Return Value

Returns true if the gamePlayerID and teamPlayerID properties are the same across all instances of this game; otherwise, false if the identifiers are unique to this game instance only.

## Mentioned in 

Protecting the player’s privacy using scoped identifiers

## Discussion

An instance is the time between when the game launches and when the game terminates.

## See Also

### Identifying the player

var gamePlayerID: String

A unique identifier for a player of the game.

var teamPlayerID: String

A unique identifier for a player of all the games that you distribute using your developer account.

let GKPlayerIDNoLongerAvailable: String

A constant for a player ID that’s no longer available.

var playerID: String

A unique identifier for a player of the game.

Deprecated

