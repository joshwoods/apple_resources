

- GameKit
- GKScore
-  report(\_:withEligibleChallenges:withCompletionHandler:) Deprecated

Type Method

# report(\_:withEligibleChallenges:withCompletionHandler:)

Submits a list of scores and all eligible challenges.

iOS 6.0–14.0DeprecatediPadOS 6.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.10–11.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
class func report(
    _ scores: [GKScore],
    withEligibleChallenges challenges: [GKChallenge],
    withCompletionHandler completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
class func report(
    _ scores: [GKScore],
    withEligibleChallenges challenges: [GKChallenge]
) async throws
```

## Parameters 

`scores`  

An array of scores to report.

`challenges`  

An array of challenges that GameKit associates with the reported scores.

`completionHandler`  

A block that GameKit calls when the download completes.

The block receives the following parameter:

*error*  
If an error occurred, this object describes the error. If the operation completed successfully, this value is `nil`.

## See Also

### Reporting a New Score

class func report([GKLeaderboardScore], withEligibleChallenges: [GKChallenge], withCompletionHandler: (((any Error)?) -> Void)?)

Submits a list of scores and all eligible challenges.

class func report([GKScore], withCompletionHandler: (((any Error)?) -> Void)?)

Reports a list of scores to Game Center

Deprecated

