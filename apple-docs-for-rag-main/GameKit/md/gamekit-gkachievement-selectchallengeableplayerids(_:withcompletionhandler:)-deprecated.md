

- GameKit
- GKAchievement
-  selectChallengeablePlayerIDs(\_:withCompletionHandler:) Deprecated

Instance Method

# selectChallengeablePlayerIDs(\_:withCompletionHandler:)

Finds the subset of players who can earn an achievement.

iOS 6.0–8.0DeprecatediPadOS 6.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

**iOS, iPadOS, Mac Catalyst, macOS, visionOS**

``` source
func selectChallengeablePlayerIDs(
    _ playerIDs: [String]?,
    withCompletionHandler completionHandler: (([String]?, (any Error)?) -> Void)? = nil
)
```

**Mac Catalyst, visionOS**

``` source
func selectChallengeablePlayerIDs(_ playerIDs: [String]?) async throws -> [String]
```

Deprecated

This method is obsolete.

## Parameters 

`playerIDs`  

An array of `NSString` objects containing a list of players. The list of players is used to find those players that are eligible to earn the achievement.

`completionHandler`  

A block to be called when the download is completed.

The block receives the following parameters:

*challengeablePlayerIDs*  
An array of player identifiers representing the players in the original array that are able to complete the challenge. If an error occurred, this parameter may be non-`nil`, in which case the array holds whatever achievement information Game Kit was able to fetch.

*error*  
If an error occurred, this object describes the error. If the operation completed successfully, this value is `nil`.

## Discussion

When this method is called, it creates a new background task to handle the request. The method then returns control to your game. Later, when the task is complete, Game Kit calls your completion handler. The completion handler is always called on the main thread.

## See Also

### Deprecated Methods

func issueChallenge(toPlayers: [String]?, message: String?)

Issues an achievement challenge to a list of players.

Deprecated

func report(completionHandler: (((any Error)?) -> Void)?)

Reports the player’s progress to Game Center.

Deprecated

