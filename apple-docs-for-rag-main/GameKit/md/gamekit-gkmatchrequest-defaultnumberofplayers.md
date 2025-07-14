

- GameKit
- GKMatchRequest
-  defaultNumberOfPlayers 

Instance Property

# defaultNumberOfPlayers

The default number of players for the match.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var defaultNumberOfPlayers: Int { get set }
```

## Discussion

GameKit uses the default number of players to present the available slots in the matchmaking user interface. The player can choose to override this to add or remove slots. If you don’t set this property, GameKit uses the value of the maxPlayers property as the default number of players.

## See Also

### Restricting the number of players

class func maxPlayersAllowedForMatch(of: GKMatchType) -> Int

Returns the maximum number of players allowed in the match request for a given match type.

enum GKMatchType

The kind of match managed by Game Center.

var minPlayers: Int

The minimum number of players that can join the match.

var maxPlayers: Int

The maximum number of players that can join the match.

