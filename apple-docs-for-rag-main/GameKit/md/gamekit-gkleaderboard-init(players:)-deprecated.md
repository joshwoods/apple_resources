

- GameKit
- GKLeaderboard
-  init(players:) Deprecated

Initializer

# init(players:)

Initializes a leaderboard request to retrieve the scores of a specific group of players.

iOS 8.0–14.0DeprecatediPadOS 8.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedmacOS 10.10–11.0DeprecatedtvOS 9.0–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–7.0Deprecated

``` source
init(players: [GKPlayer])
```

Deprecated

Use the loadEntries(for:timeScope:completionHandler:) method instead.

## Parameters 

`players`  

An array of GKPlayer objects that holds the player identifiers to retrieve.

## Return Value

An initialized leaderboard request.

## Discussion

A leaderboard object that you initialize with this method ignores the playerScope and range properties. Instead, it retrieves scores for the specific list of players whose GKPlayer objects are in the `players` parameter.

## See Also

### Deprecated initializers

init?(playerIDs: [String]?)

Initializes a leaderboard request to retrieve the scores of a specific group of players.

Deprecated

