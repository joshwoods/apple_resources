

- GameKit
- GKTurnBasedMatch
-  endTurn(withNextParticipant:match:completionHandler:) Deprecated

Instance Method

# endTurn(withNextParticipant:match:completionHandler:)

Updates the data stored on Game Center for the current match.

visionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

**visionOS, watchOS**

``` source
func endTurn(
    withNextParticipant nextParticipant: GKTurnBasedParticipant,
    match matchData: Data,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

**visionOS**

``` source
func endTurn(
    withNextParticipant nextParticipant: GKTurnBasedParticipant,
    match matchData: Data
) async throws
```

Deprecated

Use the endTurn(withNextParticipants:turnTimeout:match:completionHandler:) method instead.

## Parameters 

`nextParticipant`  

The next player in the match who needs to take an action. It must be one of the object’s stored in the match’s participants property.

`matchData`  

A serialized blob of data reflecting the game-specific state for the match. Do not pass `nil` as an argument.

`completionHandler`  

A block to be called after the data is uploaded to Game Center.

The block receives the following parameters:

*error*  
If an error occurred, this error object describes the error. If the operation was completed successfully, the value is `nil`.

## Discussion

When this method is called, it creates a new background task to handle the request. The method then returns control to your game. Later, when the task is complete, Game Kit calls your completion handler. The completion handler is always called on the main thread.

## See Also

### Deprecated Methods

func participantQuitInTurn(with: GKTurnBasedMatch.Outcome, nextParticipant: GKTurnBasedParticipant, match: Data, completionHandler: (((any Error)?) -> Void)?)

Resigns the current player from the match without ending the match.

Deprecated

func endMatchInTurn(withMatch: Data, scores: [GKScore]?, achievements: [GKAchievement]?, completionHandler: (((any Error)?) -> Void)?)

Ends the match while submitting all of the scores and achievements.

Deprecated

