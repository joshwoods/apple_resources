

- GameKit
- GKTurnBasedMatch
-  endMatchInTurn(withMatch:scores:achievements:completionHandler:) Deprecated

Instance Method

# endMatchInTurn(withMatch:scores:achievements:completionHandler:)

Ends the match while submitting all of the scores and achievements.

iOS 6.0–14.0DeprecatediPadOS 6.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.10–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
func endMatchInTurn(
    withMatch matchData: Data,
    scores: [GKScore]?,
    achievements: [GKAchievement]?,
    completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func endMatchInTurn(
    withMatch matchData: Data,
    scores: [GKScore]?,
    achievements: [GKAchievement]?
) async throws
```

Deprecated

Use the endMatchInTurn(withMatch:scores:achievements:completionHandler:) method instead.

## Parameters 

`matchData`  

A serialized blob of data reflecting the current state for the match. Do not pass `nil` as an argument.

`scores`  

An array of `GKScore` objects containing the final scores for every participant in the match.

`achievements`  

An array of `GKAchievement` objects containing the achievements acquired by each participant in the match.

`completionHandler`  

A block to be called after the scores are saved to the server.

The block receives the following parameters:

*error*  
If an error occurred, this error object describes the error. If the operation was completed successfully, the value is `nil`.

## Discussion

When this method is called, it creates a new background task to handle the request. The method then returns control to your game. Later, when the task is complete, Game Kit calls your completion handler. The completion handler is always called on the main thread.

This method ends the current match and submits scores and achievements for all of the participants. The scores can submitted to multiple leaderboards. The `GKTurnBasedMatchOutcome` status must be set for each participant before calling this method.

## See Also

### Deprecated Methods

func participantQuitInTurn(with: GKTurnBasedMatch.Outcome, nextParticipant: GKTurnBasedParticipant, match: Data, completionHandler: (((any Error)?) -> Void)?)

Resigns the current player from the match without ending the match.

Deprecated

func endTurn(withNextParticipant: GKTurnBasedParticipant, match: Data, completionHandler: (((any Error)?) -> Void)?)

Updates the data stored on Game Center for the current match.

Deprecated

