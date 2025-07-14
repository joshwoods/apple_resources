

- GameKit
- GKTurnBasedParticipant
- GKTurnBasedParticipant.Status
-  GKTurnBasedParticipant.Status.declined 

Case

# GKTurnBasedParticipant.Status.declined

The participant declines the invitation to join the match, automatically terminating the match.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
case declined
```

## See Also

### Constants

case unknown

The participant is in an unexpected state.

case invited

The participant is invited to the match, but hasn’t responded to the invitation.

case matching

The participant represents an unfilled position in the match that Game Center promises to fill when needed.

case active

The participant joins the match and is an active player.

case done

The participant leaves the match.

