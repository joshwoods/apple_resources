

- GameKit
- GKTurnBasedParticipant
-  GKTurnBasedParticipant.Status 

Enumeration

# GKTurnBasedParticipant.Status

The state the participant is in during the match.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
enum Status
```

## Mentioned in 

Starting turn-based matches and passing turns between players

## Topics

### Constants

case unknown

The participant is in an unexpected state.

case invited

The participant is invited to the match, but hasn’t responded to the invitation.

case declined

The participant declines the invitation to join the match, automatically terminating the match.

case matching

The participant represents an unfilled position in the match that Game Center promises to fill when needed.

case active

The participant joins the match and is an active player.

case done

The participant leaves the match.

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

### Retrieving Participant Details

var lastTurnDate: Date?

The date and time that this participant last took a turn in the game.

var timeoutDate: Date?

The date and time that the participant’s turn timed out.

var player: GKPlayer?

The player object containing the participant details.

var status: GKTurnBasedParticipant.Status

The status of the participant.

var playerID: String?

The player identifier for this participant.

Deprecated

