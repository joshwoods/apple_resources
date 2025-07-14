

- GameKit
- GKLeaderboard
-  isLoading Deprecated

Instance Property

# isLoading

A Boolean value that indicates whether the leaderboard object is retrieving scores.

iOS 4.1–14.0DeprecatediPadOS 4.1–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.8–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
var isLoading: Bool { get }
```

Deprecated

Use the loadEntries(for:timeScope:range:completionHandler:) method instead.

## Discussion

The value of the `loading` property is true if the leaderboard object has any pending requests for scores.

## See Also

### Deprecated properties

var category: String?

The named leaderboard to retrieve information from.

Deprecated

var identifier: String?

The named leaderboard to retrieve information from.

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

