

- GameKit
- GKScore
-  shouldSetDefaultLeaderboard Deprecated

Instance Property

# shouldSetDefaultLeaderboard

A Boolean value that indicates whether this score should also update the default leaderboard.

iOS 5.0–14.0DeprecatediPadOS 5.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.8–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
var shouldSetDefaultLeaderboard: Bool { get set }
```

## Discussion

If the value of this property is true, when the score is reported to Game Center, Game Center also updates the local player’s default leaderboard to match the value stored in the leaderboardIdentifier property of the score object. This matches the behavior of the GKLeaderboard class’s setDefault(_:withCompletionHandler:) class method. If the value of this property is false, the default leaderboard is not changed by reporting the score. The default value of this property is false.

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

func report(completionHandler: (((any Error)?) -> Void)?)

Reports a score to Game Center.

Deprecated

