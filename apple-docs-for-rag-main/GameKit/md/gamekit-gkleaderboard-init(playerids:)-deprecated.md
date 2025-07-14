

- GameKit
- GKLeaderboard
-  init(playerIDs:) Deprecated

Initializer

# init(playerIDs:)

Initializes a leaderboard request to retrieve the scores of a specific group of players.

iOS 4.1–8.0DeprecatediPadOS 4.1–8.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
init?(playerIDs: [String]?)
```

Deprecated

Use the loadEntries(for:timeScope:completionHandler:) method instead.

## Parameters 

`playerIDs`  

An array of `NSString` objects that holds the player identifier strings of the players to retrieve.

## Return Value

An initialized leaderboard request.

## Discussion

A leaderboard object that you initialize with this method ignores the playerScope and range properties. Instead, it retrieves scores for the specific list of players whose identifiers are in the `playerIDs` parameter.

## See Also

### Deprecated initializers

init(players: [GKPlayer])

Initializes a leaderboard request to retrieve the scores of a specific group of players.

Deprecated

