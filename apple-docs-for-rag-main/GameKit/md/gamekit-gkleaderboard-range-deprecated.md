

- GameKit
- GKLeaderboard
-  range Deprecated

Instance Property

# range

The numerical score rankings to return from the search.

iOS 4.0–14.0DeprecatediPadOS 4.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.8–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
var range: NSRange { get set }
```

Deprecated

Use the loadEntries(for:timeScope:range:completionHandler:) method instead.

## Discussion

GameKit ignores the range property if the leaderboard request initializes using the init(playerIDs:) method. Otherwise, the range property filters which scores to return to your game. For example, if you specify a range of `[1,10]`, when the search completes, your game receives the best ten scores. The default range is `[1,25]`.

The minimum index is `1`. The maximum length is `100`.

## See Also

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

var scores: [GKScore]?

An array of scores that contains the scores that the search returns.

Deprecated

var timeScope: GKLeaderboard.TimeScope

A filter that restricts the search to scores within a specific period of time.

Deprecated

