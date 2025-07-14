

- GameKit
- GKLeaderboard
-  baseLeaderboardID 

Instance Property

# baseLeaderboardID

The ID that Game Center uses to identify this leaderboard.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var baseLeaderboardID: String { get }
```

## Discussion

This is the same ID that App Store Connect uses to identify this leaderboard.

## See Also

### Accessing Identifier and Type Properties

var title: String?

The localized title for the leaderboard.

var type: GKLeaderboard.LeaderboardType

The type of leaderboard, classic or recurring.

enum LeaderboardType

Specifies whether a leaderboard is recurring.

var groupIdentifier: String?

The identifier for the group the leaderboard belongs to.

