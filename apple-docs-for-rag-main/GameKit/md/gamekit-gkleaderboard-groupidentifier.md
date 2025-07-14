

- GameKit
- GKLeaderboard
-  groupIdentifier 

Instance Property

# groupIdentifier

The identifier for the group the leaderboard belongs to.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var groupIdentifier: String? { get }
```

## Discussion

If you add the leaderboard to a group in App Store Connect, this property is the leaderboard group ID you enter in App Store Connect.

## See Also

### Accessing Identifier and Type Properties

var baseLeaderboardID: String

The ID that Game Center uses to identify this leaderboard.

var title: String?

The localized title for the leaderboard.

var type: GKLeaderboard.LeaderboardType

The type of leaderboard, classic or recurring.

enum LeaderboardType

Specifies whether a leaderboard is recurring.

