

- GameKit
- GKTurnBasedMatch
-  participantQuitInTurn(with:nextParticipant:match:completionHandler:) Deprecated

Instance Method

# participantQuitInTurn(with:nextParticipant:match:completionHandler:)

Resigns the current player from the match without ending the match.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

**visionOS, watchOS**

``` source
func participantQuitInTurn(
    with matchOutcome: GKTurnBasedMatch.Outcome,
    nextParticipant: GKTurnBasedParticipant,
    match matchData: Data,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

**visionOS**

``` source
func participantQuitInTurn(
    with matchOutcome: GKTurnBasedMatch.Outcome,
    nextParticipant: GKTurnBasedParticipant,
    match matchData: Data
) async throws
```

Deprecated

Use the participantQuitInTurn(with:nextParticipants:turnTimeout:match:completionHandler:) method instead.

## Parameters 

`matchOutcome`  

The end outcome of the current player in the match. Do not pass `nil` as an argument.

`nextParticipant`  

The next player in the match who needs to take an action. It must be one of the object’s stored in the match’s participants property.

`matchData`  

A serialized blob of data reflecting the game-specific state for the match.

`completionHandler`  

A block to be called after the data is uploaded to the server.

The block receives the following parameters:

*error*  
If an error occurred, this error object describes the error. If the operation was completed successfully, the value is `nil`.

## Discussion

Your game calls this method on an instance of your game that is processing the current player’s turn, but that player has left the match. For example, the player may have willingly resigned from the match or that player may have been eliminated by the other players (based on your game’s internal logic).

When this method is called, it creates a new background task to handle the request. The method then returns control to your game. Later, when the task is complete, Game Kit calls your completion handler. The completion handler is always called on the main thread.

## See Also

### Deprecated Methods

func endMatchInTurn(withMatch: Data, scores: [GKScore]?, achievements: [GKAchievement]?, completionHandler: (((any Error)?) -> Void)?)

Ends the match while submitting all of the scores and achievements.

Deprecated

func endTurn(withNextParticipant: GKTurnBasedParticipant, match: Data, completionHandler: (((any Error)?) -> Void)?)

Updates the data stored on Game Center for the current match.

Deprecated

