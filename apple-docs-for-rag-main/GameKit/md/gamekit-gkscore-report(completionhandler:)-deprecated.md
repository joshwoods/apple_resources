

- GameKit
- GKScore
-  report(completionHandler:) Deprecated

Instance Method

# report(completionHandler:)

Reports a score to Game Center.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

**macOS, visionOS, watchOS**

``` source
func report(completionHandler: (((any Error)?) -> Void)? = nil)
```

**visionOS**

``` source
func report() async throws
```

## Parameters 

`completionHandler`  

A block to be called after the score is reported.

The block receives the following parameter:

*error*  
If an error occurred, this parameter holds an error object that describes the problem. If the score was successfully reported, this parameter’s value is `nil`.

## Discussion

The `value` property must be set before calling this method.

When this method is called, it creates a new background task to handle the request. The method then returns control to your game. Later, when the task is complete, GameKit calls your completion handler. The completion handler is always called on the main thread.

## See Also

### Deprecated Methods and Properties

var category: String?

The leaderboard that this score belongs to.

Deprecated

var context: UInt64

An integer value used by your game.

Deprecated

var date: Date

The date and time when the score was earned.

Deprecated

var formattedValue: String?

Returns the player’s score as a localized string.

Deprecated

var leaderboardIdentifier: String

The identifier for the leaderboard.

Deprecated

var player: GKPlayer

The player who earned the score.

Deprecated

var rank: Int

The position of the score in the results of a leaderboard search.

Deprecated

var value: Int64

The score earned by the player.

Deprecated

var shouldSetDefaultLeaderboard: Bool

A Boolean value that indicates whether this score should also update the default leaderboard.

Deprecated

init(leaderboardIdentifier: String)

Returns an initialized score object using the local player and the current date.

Deprecated

init(leaderboardIdentifier: String, player: GKPlayer)

Returns an initialized score object for the specified leaderboard and player.

Deprecated

init(category: String?)

Returns an initialized score object.

Deprecated

init?(leaderboardIdentifier: String, forPlayer: String)

Returns an initialized score object for the specified leaderboard and player.

Deprecated

func issueChallenge(toPlayers: [String]?, message: String?)

Issues a score challenge to a set of players.

Deprecated

var playerID: String?

The player identifier for the player that earned the score.

Deprecated

