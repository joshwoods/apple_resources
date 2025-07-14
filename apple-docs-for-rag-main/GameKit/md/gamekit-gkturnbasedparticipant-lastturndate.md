

- GameKit
- GKTurnBasedParticipant
-  lastTurnDate 

Instance Property

# lastTurnDate

The date and time that this participant last took a turn in the game.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var lastTurnDate: Date? { get }
```

## Discussion

This property is invalid until the participant takes their first turn.

## See Also

### Retrieving Participant Details

var timeoutDate: Date?

The date and time that the participant’s turn timed out.

var player: GKPlayer?

The player object containing the participant details.

var status: GKTurnBasedParticipant.Status

The status of the participant.

enum Status

The state the participant is in during the match.

var playerID: String?

The player identifier for this participant.

Deprecated

