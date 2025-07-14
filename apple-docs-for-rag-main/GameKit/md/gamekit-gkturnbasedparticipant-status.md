

- GameKit
- GKTurnBasedParticipant
-  status 

Instance Property

# status

The status of the participant.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var status: GKTurnBasedParticipant.Status { get }
```

## Mentioned in 

Starting turn-based matches and passing turns between players

## See Also

### Retrieving Participant Details

var lastTurnDate: Date?

The date and time that this participant last took a turn in the game.

var timeoutDate: Date?

The date and time that the participant’s turn timed out.

var player: GKPlayer?

The player object containing the participant details.

enum Status

The state the participant is in during the match.

var playerID: String?

The player identifier for this participant.

Deprecated

