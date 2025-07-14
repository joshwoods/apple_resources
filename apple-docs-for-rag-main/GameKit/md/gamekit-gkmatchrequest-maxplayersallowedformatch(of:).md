

- GameKit
- GKMatchRequest
-  maxPlayersAllowedForMatch(of:) 

Type Method

# maxPlayersAllowedForMatch(of:)

Returns the maximum number of players allowed in the match request for a given match type.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class func maxPlayersAllowedForMatch(of matchType: GKMatchType) -> Int
```

## Parameters 

`matchType`  

The kind of match.

## Return Value

The maximum number of allowed players.

## Mentioned in 

Starting turn-based matches and passing turns between players

Finding multiple players for a game

## Discussion

For peer-to-peer, hosted, and turn-based matches, the maximum number of players is `16`.

## See Also

### Restricting the number of players

enum GKMatchType

The kind of match managed by Game Center.

var minPlayers: Int

The minimum number of players that can join the match.

var maxPlayers: Int

The maximum number of players that can join the match.

var defaultNumberOfPlayers: Int

The default number of players for the match.

