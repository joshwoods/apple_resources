

- GameKit
- GKLeaderboard
-  GKLeaderboard.LeaderboardType 

Enumeration

# GKLeaderboard.LeaderboardType

Specifies whether a leaderboard is recurring.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
enum LeaderboardType
```

## Topics

### Constants

case classic

A leaderboard that never expires, showing all-time rankings of all players.

case recurring

A leaderboard that recurs, allowing players a fresh start to compete and earn higher ranks in each ocurrence.

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

### Accessing Identifier and Type Properties

var baseLeaderboardID: String

The ID that Game Center uses to identify this leaderboard.

var title: String?

The localized title for the leaderboard.

var type: GKLeaderboard.LeaderboardType

The type of leaderboard, classic or recurring.

var groupIdentifier: String?

The identifier for the group the leaderboard belongs to.

