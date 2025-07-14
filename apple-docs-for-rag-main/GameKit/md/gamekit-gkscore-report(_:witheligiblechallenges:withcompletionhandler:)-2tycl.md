

- GameKit
- GKScore
-  report(\_:withEligibleChallenges:withCompletionHandler:) 

Type Method

# report(\_:withEligibleChallenges:withCompletionHandler:)

Submits a list of scores and all eligible challenges.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
class func report(
    _ scores: [GKLeaderboardScore],
    withEligibleChallenges challenges: [GKChallenge],
    withCompletionHandler completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
class func report(
    _ scores: [GKLeaderboardScore],
    withEligibleChallenges challenges: [GKChallenge]
) async throws
```

## Parameters 

`scores`  

An array of scores to report.

`challenges`  

An array of challenges that GameKit associates with the reported scores.

`completionHandler`  

A block that GameKit calls when this method completes.

The block receives the following parameter:

*error*  
If an error occurs, this object describes the error. If the operation completed successfully, this value is `nil`.

## See Also

### Reporting a New Score

class func report([GKScore], withCompletionHandler: (((any Error)?) -> Void)?)

Reports a list of scores to Game Center

Deprecated

class func report([GKScore], withEligibleChallenges: [GKChallenge], withCompletionHandler: (((any Error)?) -> Void)?)

Submits a list of scores and all eligible challenges.

Deprecated

