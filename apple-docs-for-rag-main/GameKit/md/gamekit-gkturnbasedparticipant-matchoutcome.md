

- GameKit
- GKTurnBasedParticipant
-  matchOutcome 

Instance Property

# matchOutcome

The conclusion or results of a participant in a match.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var matchOutcome: GKTurnBasedMatch.Outcome { get set }
```

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

Initially, GameKit sets this property to GKTurnBasedMatch.Outcome.none. Then before a player forfeits a match or you end a match, set this property to a value that reflects the participant’s outcome. Optionally, set this property to a custom value using an `OR` operation that fits in the range specified by the GKTurnBasedMatch.Outcome.customRange enumeration case.

## See Also

### Setting Participant Outcomes

enum Outcome

The state of a participant when they forfeit a match or when a match ends.

