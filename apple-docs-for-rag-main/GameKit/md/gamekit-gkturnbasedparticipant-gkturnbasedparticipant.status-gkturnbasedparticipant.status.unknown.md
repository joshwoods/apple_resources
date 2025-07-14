

- GameKit
- GKTurnBasedParticipant
- GKTurnBasedParticipant.Status
-  GKTurnBasedParticipant.Status.unknown 

Case

# GKTurnBasedParticipant.Status.unknown

The participant is in an unexpected state.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
case unknown
```

## See Also

### Constants

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

