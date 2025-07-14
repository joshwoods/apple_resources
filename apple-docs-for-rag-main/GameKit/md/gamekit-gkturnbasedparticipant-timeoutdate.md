

- GameKit
- GKTurnBasedParticipant
-  timeoutDate 

Instance Property

# timeoutDate

The date and time that the participant’s turn timed out.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var timeoutDate: Date? { get }
```

## Discussion

This property is `nil` when the participant takes a turn that doesn’t time out.

## See Also

### Retrieving Participant Details

var lastTurnDate: Date?

The date and time that this participant last took a turn in the game.

var player: GKPlayer?

The player object containing the participant details.

var status: GKTurnBasedParticipant.Status

The status of the participant.

enum Status

The state the participant is in during the match.

var playerID: String?

The player identifier for this participant.

Deprecated

