

- GameKit
- GKScore
-  init(leaderboardIdentifier:forPlayer:) Deprecated

Initializer

# init(leaderboardIdentifier:forPlayer:)

Returns an initialized score object for the specified leaderboard and player.

iOS 7.0–8.0DeprecatediPadOS 7.0–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.9–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
init?(
    leaderboardIdentifier identifier: String,
    forPlayer playerID: String
)
```

## Parameters 

`identifier`  

Identifies the leaderboard that the score is being sent to.

`playerID`  

The identifier of the player who’s score is being initialized.

## Return Value

An initialized score object, or `nil` if an error occurred.

## Discussion

Your game explicitly allocates and initializes a score object using the designated player and current date when it needs to report a new score to Game Center.

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

func issueChallenge(toPlayers: [String]?, message: String?)

Issues a score challenge to a set of players.

Deprecated

var playerID: String?

The player identifier for the player that earned the score.

Deprecated

func report(completionHandler: (((any Error)?) -> Void)?)

Reports a score to Game Center.

Deprecated

