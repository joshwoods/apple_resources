

- GameKit
- GKMatchRequest
-  minPlayers 

Instance Property

# minPlayers

The minimum number of players that can join the match.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var minPlayers: Int { get set }
```

## Mentioned in 

Finding players using matchmaking rules

Finding multiple players for a game

## Discussion

The possible values range from `2` to the value returned by the maxPlayersAllowedForMatch(of:) method. To set the maximum number of players, use the maxPlayers property.

If you use matchmaking rules, the rule set’s `minPlayers` field constrains this value. Set this property to a value in the range of the rule set’s `minPlayers` and `maxPlayers` fields. The default value is the rule set’s `minPlayers` field.

## See Also

### Related Documentation

Create a rule set

Create a rule set to contain matchmaking rules and teams.

### Restricting the number of players

class func maxPlayersAllowedForMatch(of: GKMatchType) -> Int

Returns the maximum number of players allowed in the match request for a given match type.

enum GKMatchType

The kind of match managed by Game Center.

var maxPlayers: Int

The maximum number of players that can join the match.

var defaultNumberOfPlayers: Int

The default number of players for the match.

