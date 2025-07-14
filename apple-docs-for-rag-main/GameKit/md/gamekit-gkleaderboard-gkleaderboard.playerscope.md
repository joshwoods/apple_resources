

- GameKit
- GKLeaderboard
-  GKLeaderboard.PlayerScope 

Enumeration

# GKLeaderboard.PlayerScope

Specifies the type of players for filtering data.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
enum PlayerScope
```

## Topics

### Constants

case global

Loads data for all players of the game.

case friendsOnly

Loads only data for friends of the local player.

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

enum TimeScope

Specifies the time period for filtering data.

class Entry

Information about a single score by a player on a leaderboard.

