

- GameKit
- GKTurnBasedParticipant
-  player 

Instance Property

# player

The player object containing the participant details.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var player: GKPlayer? { get }
```

## Mentioned in 

Starting turn-based matches and passing turns between players

## Discussion

This property is `nil` if this slot isn’t filled yet — for example, when Game Center uses automatch to fill this slot.

## See Also

### Retrieving Participant Details

var lastTurnDate: Date?

The date and time that this participant last took a turn in the game.

var timeoutDate: Date?

The date and time that the participant’s turn timed out.

var status: GKTurnBasedParticipant.Status

The status of the participant.

enum Status

The state the participant is in during the match.

var playerID: String?

The player identifier for this participant.

Deprecated

