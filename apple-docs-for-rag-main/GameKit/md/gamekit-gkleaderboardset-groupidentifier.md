

- GameKit
- GKLeaderboardSet
-  groupIdentifier 

Instance Property

# groupIdentifier

The identifier for the group that the leaderboard set belongs to.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
var groupIdentifier: String? { get }
```

## Discussion

GameKit sets this property when the leaderboard set is part of a game group, and it calls `loadLeaderboardSetsWithCompletionHandler:` for leaderboards that support game groups.

## See Also

### Accessing Properties

var title: String

The localized title for the leaderboard set.

var identifier: String?

The identifier for the leaderboard set.

