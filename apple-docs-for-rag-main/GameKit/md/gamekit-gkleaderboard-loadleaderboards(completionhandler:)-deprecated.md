

- GameKit
- GKLeaderboard
-  loadLeaderboards(completionHandler:) Deprecated

Type Method

# loadLeaderboards(completionHandler:)

Loads a list of leaderboards from Game Center.

iOS 6.0–14.0DeprecatediPadOS 6.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.8–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
class func loadLeaderboards(completionHandler: (([GKLeaderboard]?, (any Error)?) -> Void)? = nil)
```

``` source
class func loadLeaderboards() async throws -> [GKLeaderboard]
```

Deprecated

Use the loadLeaderboards(IDs:completionHandler:) method instead.

## Parameters 

`completionHandler`  

A block to call when loading the leaderboards.

The block receives the following parameters:

*leaderboards*  
An array of `GKLeaderboard` objects that provides the leaderboards for your game. If an error occurs, this value may be non-`nil`. In this case, the array holds whatever data GameKit downloads before the error occurs.

*error*  
If an error occurs, this error object describes the error. If the operation completes successfully, the value is `nil`.

## Discussion

Use this class method to retrieve the list of leaderboards you configure in App Store Connect. Use the properties of each leaderboard object, especially the category and title properties, to learn more about the leaderboard.

```
- (void) loadLeaderboardInfo
{
    [GKLeaderboard loadLeaderboardsWithCompletionHandler:^(NSArray *leaderboards, NSError *error) {
        self.leaderboards = leaderboards;
     }];
}
```

When you call this method, it creates a new background task to handle the request. The method then returns control to your game. When the task is complete, GameKit calls your completion handler on the main thread.

## See Also

### Deprecated methods

class func setDefault(String?, withCompletionHandler: (((any Error)?) -> Void)?)

Sets the default leaderboard for the local player.

Deprecated

class func loadCategories(completionHandler: (([String]?, [String]?, (any Error)?) -> Void)?)

Loads the list of leaderboard categories along with their corresponding localized titles.

Deprecated

func loadScores(completionHandler: (([GKScore]?, (any Error)?) -> Void)?)

Retrieves a set of scores from Game Center.

Deprecated

