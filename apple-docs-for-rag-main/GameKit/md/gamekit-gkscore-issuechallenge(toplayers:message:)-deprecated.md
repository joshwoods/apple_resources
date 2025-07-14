

- GameKit
- GKScore
-  issueChallenge(toPlayers:message:) Deprecated

Instance Method

# issueChallenge(toPlayers:message:)

Issues a score challenge to a set of players.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func issueChallenge(
    toPlayers playerIDs: [String]?,
    message: String?
)
```

## Parameters 

`playerIDs`  

The identifiers for the players to challenge. Because Game Center limits the number of players in a challenge request to 10, the maximum size of this array is 10.

`message`  

A text message to display to the players.

## Discussion

Set up your game to issue a challenge request only in direct response to a player action. That is, your game provides a user interface that allows the player to choose to issue a challenge and choose which friends receive the challenge, and only issue a challenge when the player wishes to do so.

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

var playerID: String?

The player identifier for the player that earned the score.

Deprecated

func report(completionHandler: (((any Error)?) -> Void)?)

Reports a score to Game Center.

Deprecated

