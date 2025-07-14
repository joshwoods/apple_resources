

- GameKit
- GKAchievement
-  Deprecated Symbols 

API Collection

# Deprecated Symbols

Review unsupported symbols and their replacements.

## Topics

### Deprecated Initializers

init?(identifier: String?, forPlayer: String)

Initializes an achievement for a specific player.

Deprecated

### Deprecated Methods

func issueChallenge(toPlayers: [String]?, message: String?)

Issues an achievement challenge to a list of players.

Deprecated

func report(completionHandler: (((any Error)?) -> Void)?)

Reports the player’s progress to Game Center.

Deprecated

func selectChallengeablePlayerIDs([String]?, withCompletionHandler: (([String]?, (any Error)?) -> Void)?)

Finds the subset of players who can earn an achievement.

Deprecated

### Deprecated Properties

var isHidden: Bool

A Boolean value that indicates whether the system hides this achievement from the player.

Deprecated

var playerID: String?

A string that identifies the player who earned the achievement.

Deprecated

