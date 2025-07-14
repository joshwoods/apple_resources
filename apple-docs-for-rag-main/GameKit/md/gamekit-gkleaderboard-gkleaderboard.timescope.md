

- GameKit
- GKLeaderboard
-  GKLeaderboard.TimeScope 

Enumeration

# GKLeaderboard.TimeScope

Specifies the time period for filtering data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
enum TimeScope
```

## Topics

### Constants

case today

Loads data for the past 24 hours.

case week

Loads data for the past week.

case allTime

Loads a player’s best score.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Loading Scores

func loadEntries(for: GKLeaderboard.PlayerScope, timeScope: GKLeaderboard.TimeScope, range: NSRange, completionHandler: (GKLeaderboard.Entry?, [GKLeaderboard.Entry]?, Int, (any Error)?) -> Void)

Returns the scores for the local player and other players for the specified type of player, time period, and ranks.

func loadEntries(for: [GKPlayer], timeScope: GKLeaderboard.TimeScope, completionHandler: (GKLeaderboard.Entry?, [GKLeaderboard.Entry]?, (any Error)?) -> Void)

Returns the scores for the local player and other players for the specified time period.

enum PlayerScope

Specifies the type of players for filtering data.

class Entry

Information about a single score by a player on a leaderboard.

