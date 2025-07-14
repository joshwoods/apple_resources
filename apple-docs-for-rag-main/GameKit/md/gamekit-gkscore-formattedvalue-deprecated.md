

- GameKit
- GKScore
-  formattedValue Deprecated

Instance Property

# formattedValue

Returns the player’s score as a localized string.

iOS 4.1–14.0DeprecatediPadOS 4.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.8–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
var formattedValue: String? { get }
```

## Discussion

This property is invalid on a newly initialized score object. On a score returned from GameKit, it contains a formatted string based on the player’s score. You determine how a score is formatted when you define the leaderboard in App Store Connect.

Never convert the `value` property into a string directly; always use this method to receive the formatted string.

Important

You may be tempted to write your own formatting code rather than using the `formattedValue` property. Do not do this. Using the built-in support makes it easy to localize the score value into other languages, and provides a string that is consistent with the presentation of your scores in the Game Center app.

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

func report(completionHandler: (((any Error)?) -> Void)?)

Reports a score to Game Center.

Deprecated

