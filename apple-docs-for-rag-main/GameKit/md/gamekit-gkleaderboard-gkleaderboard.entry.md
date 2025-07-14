

- GameKit
- GKLeaderboard
-  GKLeaderboard.Entry 

Class

# GKLeaderboard.Entry

Information about a single score by a player on a leaderboard.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
class Entry
```

## Mentioned in 

Encourage progress and competition with leaderboards

## Topics

### Accessing Properties

var context: Int

An integer value that your game uses.

var date: Date

The date and time when the player earns the score.

var formattedScore: String

The player’s score as a localized string.

var player: GKPlayer

The player who earns the score.

var rank: Int

The position of the score in the results of a leaderboard search.

var score: Int

The score that the player earns.

### Presenting Challenges

func challengeComposeController(withMessage: String?, players: [GKPlayer]?, completion: GKChallengeComposeHandler?) -> UIViewController

Provides a challenge compose view controller with preselected player identifiers and a preformatted, player-editable message.

typealias GKChallengeComposeHandler

A completion block that provides information about the player who issues a challenge and the players who receive it.

func challengeComposeController(withMessage: String?, players: [GKPlayer]?, completionHandler: GKChallengeComposeCompletionBlock?) -> UIViewController

Provides a challenge compose view controller with preselected player identifiers and a preformatted, player-editable message.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Loading Scores

func loadEntries(for: GKLeaderboard.PlayerScope, timeScope: GKLeaderboard.TimeScope, range: NSRange, completionHandler: (GKLeaderboard.Entry?, [GKLeaderboard.Entry]?, Int, (any Error)?) -> Void)

Returns the scores for the local player and other players for the specified type of player, time period, and ranks.

func loadEntries(for: [GKPlayer], timeScope: GKLeaderboard.TimeScope, completionHandler: (GKLeaderboard.Entry?, [GKLeaderboard.Entry]?, (any Error)?) -> Void)

Returns the scores for the local player and other players for the specified time period.

enum PlayerScope

Specifies the type of players for filtering data.

enum TimeScope

Specifies the time period for filtering data.

