

- GameKit
- GKLeaderboard
-  setDefault(\_:withCompletionHandler:) Deprecated

Type Method

# setDefault(\_:withCompletionHandler:)

Sets the default leaderboard for the local player.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

**macOS, visionOS, watchOS**

``` source
class func setDefault(
    _ leaderboardIdentifier: String?,
    withCompletionHandler completionHandler: (((any Error)?) -> Void)? = nil
)
```

**visionOS**

``` source
class func setDefault(_ leaderboardIdentifier: String?) async throws
```

Deprecated

Use the setDefaultLeaderboardIdentifier(_:completionHandler:) method instead.

## Parameters 

`leaderboardIdentifier`  

The named leaderboard that is the new default leaderboard for the local player.

`completionHandler`  

A block to call after retrieving scores from the server.

The block receives the following parameter:

*error*  
If an error occurs, this error object describes the error. If the operation completes successfully, the value is `nil`.

## Discussion

GameKit uses the default leaderboard whenever your game uses a GKScore object to report a score to Game Center without explicitly setting the score object’s category property. You normally set the default leaderboard in App Store Connect. However, your game can use this class method to override the default leaderboard that appears for the local player. Game Center stores this information for each player.

When you call this method, it creates a new background task to handle the request. The method then returns control to your game. When the task completes, GameKit calls your completion handler on the main thread.

If an error occurs and it’s a network error, periodically resend the request until it completes.

## See Also

### Deprecated methods

class func loadCategories(completionHandler: (([String]?, [String]?, (any Error)?) -> Void)?)

Loads the list of leaderboard categories along with their corresponding localized titles.

Deprecated

class func loadLeaderboards(completionHandler: (([GKLeaderboard]?, (any Error)?) -> Void)?)

Loads a list of leaderboards from Game Center.

Deprecated

func loadScores(completionHandler: (([GKScore]?, (any Error)?) -> Void)?)

Retrieves a set of scores from Game Center.

Deprecated

