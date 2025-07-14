

- GameKit
- GKTurnBasedParticipant
-  playerID Deprecated

Instance Property

# playerID

The player identifier for this participant.

iOS 5.0–8.0DeprecatediPadOS 5.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
var playerID: String? { get }
```

Deprecated

User player instead.

## Discussion

This property is `nil` if this slot isn’t filled yet — for example, when Game Center uses automatch to fill this slot.

## See Also

### Retrieving Participant Details

var lastTurnDate: Date?

The date and time that this participant last took a turn in the game.

var timeoutDate: Date?

The date and time that the participant’s turn timed out.

var player: GKPlayer?

The player object containing the participant details.

var status: GKTurnBasedParticipant.Status

The status of the participant.

enum Status

The state the participant is in during the match.

