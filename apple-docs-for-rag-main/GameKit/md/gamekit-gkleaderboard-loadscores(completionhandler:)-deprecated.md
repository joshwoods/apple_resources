

- GameKit
- GKLeaderboard
-  loadScores(completionHandler:) Deprecated

Instance Method

# loadScores(completionHandler:)

Retrieves a set of scores from Game Center.

iOS 4.0–14.0DeprecatediPadOS 4.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.8–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
func loadScores(completionHandler: (([GKScore]?, (any Error)?) -> Void)? = nil)
```

Deprecated

Use the loadEntries(for:timeScope:range:completionHandler:) method instead.

## Parameters 

`completionHandler`  

A block to call after retrieving the scores from the server.

The block receives the following parameters:

*scores*  
An array of `GKScore` objects that holds the requested scores. If an error occurs, this value may be non-`nil`. In this case, the array holds whatever score data GameKit retrieves from Game Center before the error occurs.

*error*  
If an error occurs, this error object describes the error. If the operation completes successfully, the value is `nil`.

## Discussion

When you call this method, it creates a new background task to handle the request. The method then returns control to your game. When the task completes, GameKit calls your completion handler on the main thread.

The code below shows an example leaderboard data query. The method for this query initializes a new leaderboard object and configures the playerScope, timeScope, and range properties to retrieve the top ten scores for today.

```
- (void) retrieveTopTenScores
{
    GKLeaderboard *leaderboardRequest = [[GKLeaderboard alloc] init];
    if (leaderboardRequest != nil)
    {
        leaderboardRequest.playerScope = GKLeaderboardPlayerScopeGlobal;
        leaderboardRequest.timeScope = GKLeaderboardTimeScopeToday;
        leaderboardRequest.identifier = @"Combined.LandMaps"
        leaderboardRequest.range = NSMakeRange(1,10);
        [leaderboardRequest loadScoresWithCompletionHandler: ^(NSArray *scores, NSError *error) {
            if (error != nil)
            {
                // Handle the error.
            }
            if (scores != nil)
            {
                // Process the score information.
            }
            }];
    }
}
```

You can create a leaderboard request that retrieves scores for a specific list of players.

```
- (void) receiveMatchBestScores: (GKMatch*) match
{
    GKLeaderboard *leaderboardRequest = [[GKLeaderboard alloc] initWithPlayers: match.players];
        leaderboardRequest.timeScope = GKLeaderboardTimeScopeAllTime;
        leaderboardRequest.identifier = @"Combined.LandMaps"
        leaderboardRequest.range = NSMakeRange(1,10);
    if (query != nil)
    {
        [query loadScoresWithCompletionHandler: ^(NSArray *scores, NSError *error) {
            if (error != nil)
            {
                // Handle the error.
            }
            if (scores != nil)
            {
                // Process the score information.
            }
        }];
    }
}
```

You can call this method multiple times. Each call represents a different query against the scores stored in Game Center. If you post multiple load operations using the same leaderboard object, any properties that update by loading scores reflect the most recent query that completes. The order that achievement queries process is arbitrary.

## See Also

### Deprecated methods

class func setDefault(String?, withCompletionHandler: (((any Error)?) -> Void)?)

Sets the default leaderboard for the local player.

Deprecated

class func loadCategories(completionHandler: (([String]?, [String]?, (any Error)?) -> Void)?)

Loads the list of leaderboard categories along with their corresponding localized titles.

Deprecated

class func loadLeaderboards(completionHandler: (([GKLeaderboard]?, (any Error)?) -> Void)?)

Loads a list of leaderboards from Game Center.

Deprecated

