

- GameKit
- GKTurnBasedMatch
-  GKTurnBasedMatch.Outcome 

Enumeration

# GKTurnBasedMatch.Outcome

The state of a participant when they forfeit a match or when a match ends.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
enum Outcome
```

## Topics

### Outcomes

case none

The participant doesn’t reach an outcome.

case quit

The participant forfeits the match.

case won

The participant wins the match.

case lost

The participant loses the match.

case tied

The participant ties the match.

case timeExpired

The match ends because the time limit expires.

case first

The participant finishes in first place.

case second

The participant finishes in second place.

case third

The participant finishes in third place.

case fourth

The participant finishes in fourth place.

case customRange

The participant reaches a game-specific outcome.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Forfeiting a Match

func participantQuitInTurn(with: GKTurnBasedMatch.Outcome, nextParticipants: [GKTurnBasedParticipant], turnTimeout: TimeInterval, match: Data, completionHandler: (((any Error)?) -> Void)?)

Forfeits the match on behalf of the local player when it’s their turn.

func participantQuitOutOfTurn(with: GKTurnBasedMatch.Outcome, withCompletionHandler: (((any Error)?) -> Void)?)

Forfeits the match on behalf of the local player when it’s not their turn.

