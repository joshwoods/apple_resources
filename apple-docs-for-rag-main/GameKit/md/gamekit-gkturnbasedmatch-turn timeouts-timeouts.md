

- GameKit
- GKTurnBasedMatch
-  Turn Timeouts 

API Collection

# Turn Timeouts

A timeout for a player to take their turn.

## Topics

### Timeouts

var GKTurnTimeoutDefault: TimeInterval

A one-week time limit to take a turn.

var GKTurnTimeoutNone: TimeInterval

No timeout to take a turn.

## See Also

### Ending Turns and Saving Data

func endTurn(withNextParticipants: [GKTurnBasedParticipant], turnTimeout: TimeInterval, match: Data, completionHandler: (((any Error)?) -> Void)?)

Passes the turn from the current participant to the next participant.

func saveCurrentTurn(withMatch: Data, completionHandler: (((any Error)?) -> Void)?)

Saves your match data in Game Center without ending the turn.

