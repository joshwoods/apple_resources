

- GameKit
- GKTurnBasedMatch
-  currentParticipant 

Instance Property

# currentParticipant

The participant whose turn it is.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var currentParticipant: GKTurnBasedParticipant? { get }
```

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

You can only update the match data when the current participant is the local player.

## See Also

### Retrieving Match Details

var matchID: String

A unique identifier for the turn-based match.

var creationDate: Date

The date that Game Center created the match.

var participants: [GKTurnBasedParticipant]

The players that participate in a turn-based match.

var status: GKTurnBasedMatch.Status

The state of the match, such as whether the match is open or has ended.

enum Status

The states of a match from when it’s created to when it ends.

var matchData: Data?

The game-specific data that you store in Game Center and pass between participants through a match object.

var matchDataMaximumSize: Int

The maximum size of the match data.

func loadMatchData(completionHandler: ((Data?, (any Error)?) -> Void)?)

Fetches your game-specific data that you store in Game Center when ending a turn, saving a turn, or leaving a match.

