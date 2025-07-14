

- GameKit
- GKLeaderboard
-  category Deprecated

Instance Property

# category

The named leaderboard to retrieve information from.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var category: String? { get set }
```

Deprecated

Use the loadEntries(for:timeScope:range:completionHandler:) method instead.

## Discussion

If non-`nil`, Game Center only returns scores from the matching leaderboard. If `nil`, Game Center searches all previous scores of the game. The default is `nil`.

## See Also

### Deprecated properties

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

