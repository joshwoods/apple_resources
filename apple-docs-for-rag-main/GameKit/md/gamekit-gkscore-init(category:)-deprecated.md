

- GameKit
- GKScore
-  init(category:) Deprecated

Initializer

# init(category:)

Returns an initialized score object.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
init(category: String?)
```

## Parameters 

`category`  

An identifier for a specific leaderboard you’ve configured in App Store Connect. Must not be `nil`.

## Return Value

An initialized score object, or `nil` if an error occurred.

## Discussion

Your game explicitly allocates and initializes a score object when it needs to report a new score to Game Center.

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

