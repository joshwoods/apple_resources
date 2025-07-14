

- GameKit
- GKTurnBasedParticipant
- GKTurnBasedParticipant.Status
-  GKTurnBasedParticipant.Status.active 

Case

# GKTurnBasedParticipant.Status.active

The participant joins the match and is an active player.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
case active
```

## Mentioned in 

Starting turn-based matches and passing turns between players

## See Also

### Constants

case unknown

The participant is in an unexpected state.

case invited

The participant is invited to the match, but hasn’t responded to the invitation.

case declined

The participant declines the invitation to join the match, automatically terminating the match.

case matching

The participant represents an unfilled position in the match that Game Center promises to fill when needed.

case done

The participant leaves the match.

