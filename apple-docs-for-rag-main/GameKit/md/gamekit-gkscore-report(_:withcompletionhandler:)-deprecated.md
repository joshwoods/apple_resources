

- GameKit
- GKScore
-  report(\_:withCompletionHandler:) Deprecated

Type Method

# report(\_:withCompletionHandler:)

Reports a list of scores to Game Center

iOS 6.0–14.0DeprecatediPadOS 6.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.8–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
class func report(
    _ scores: [GKScore],
    withCompletionHandler completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
class func report(_ scores: [GKScore]) async throws
```

## Parameters 

`scores`  

An array of scores to report to Game Center.

`completionHandler`  

A block that GameKit calls when it reports the scores.

The block receives the following parameter:

*error*  
If an error occurred, this parameter holds an error object that describes the problem. If the score was successfully reported, this parameter’s value is `nil`.

## Discussion

Use this class method whenever you need to submit scores to Game Center, whether you are reporting a single score or multiple scores. The method runs through the array of `GKScore` objects, submitting scores one at a time.

report(_:withCompletionHandler:) provides a sample method to report a score. The `GKScore` object is initialized with the leaderboard ID for the leaderboard it reports its score to and then the value and context for the score are assigned. The leaderboard ID must be the identifier for a leaderboard you configured in App Store Connect. Scores are always reported for the current local player and never for friends.

```
- (void) reportScore: (int64_t) score forLeaderboardID: (NSString*) identifier
{
    GKScore *scoreReporter = [[GKScore alloc] initWithLeaderboardIdentifier: identifier];
    scoreReporter.value = score;
    scoreReporter.context = 0;

    NSArray *scores = @[scoreReporter];
    [GKScore reportScores:scores withCompletionHandler:^(NSError *error) {
    //Do something interesting here.
    }];
}
```

## See Also

### Reporting a New Score

class func report([GKLeaderboardScore], withEligibleChallenges: [GKChallenge], withCompletionHandler: (((any Error)?) -> Void)?)

Submits a list of scores and all eligible challenges.

class func report([GKScore], withEligibleChallenges: [GKChallenge], withCompletionHandler: (((any Error)?) -> Void)?)

Submits a list of scores and all eligible challenges.

Deprecated

