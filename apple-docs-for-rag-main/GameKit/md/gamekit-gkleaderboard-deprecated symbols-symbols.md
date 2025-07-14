

- GameKit
- GKLeaderboard
-  Deprecated symbols 

API Collection

# Deprecated symbols

Review unsupported symbols and their replacements.

## Topics

### Deprecated initializers

init?(playerIDs: [String]?)

Initializes a leaderboard request to retrieve the scores of a specific group of players.

Deprecated

init(players: [GKPlayer])

Initializes a leaderboard request to retrieve the scores of a specific group of players.

Deprecated

### Deprecated properties

var category: String?

The named leaderboard to retrieve information from.

Deprecated

var identifier: String?

The named leaderboard to retrieve information from.

Deprecated

var isLoading: Bool

A Boolean value that indicates whether the leaderboard object is retrieving scores.

Deprecated

var localPlayerScore: GKScore?

The score that the local player earns.

Deprecated

var maxRange: Int

The size of the leaderboard.

Deprecated

var playerScope: GKLeaderboard.PlayerScope

A filter that restricts the search to a subset of the players in Game Center.

Deprecated

var range: NSRange

The numerical score rankings to return from the search.

Deprecated

var scores: [GKScore]?

An array of scores that contains the scores that the search returns.

Deprecated

var timeScope: GKLeaderboard.TimeScope

A filter that restricts the search to scores within a specific period of time.

Deprecated

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

func loadScores(completionHandler: (([GKScore]?, (any Error)?) -> Void)?)

Retrieves a set of scores from Game Center.

Deprecated

