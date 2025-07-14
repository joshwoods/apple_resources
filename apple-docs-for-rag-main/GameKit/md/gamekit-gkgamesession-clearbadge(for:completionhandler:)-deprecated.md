

- GameKit
- GKGameSession
-  clearBadge(for:completionHandler:) Deprecated

Instance Method

# clearBadge(for:completionHandler:)

Clears the badge from the designated players.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func clearBadge(
    for players: [GKCloudPlayer],
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func clearBadge(for players: [GKCloudPlayer]) async throws
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`players`  

An array of GKCloudPlayers identifying the players that are to have their badge removed.

`completionHandler`  

A block that is called after the badges have been removed from the players.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is nil. See `GameKit Constants` for a list of error codes specific to GameKit.

## See Also

### Communicating Between Players

var badgedPlayers: [GKCloudPlayer]

An array containing all of the currently badged players.

Deprecated

func sendMessage(withLocalizedFormatKey: String, arguments: [String], data: Data?, to: [GKCloudPlayer], badgePlayers: Bool, completionHandler: ((any Error)?) -> Void)

Sends a message to players in a game session.

Deprecated

