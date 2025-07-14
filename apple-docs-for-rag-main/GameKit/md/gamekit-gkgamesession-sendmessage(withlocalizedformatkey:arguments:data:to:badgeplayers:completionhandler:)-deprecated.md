

- GameKit
- GKGameSession
-  sendMessage(withLocalizedFormatKey:arguments:data:to:badgePlayers:completionHandler:) Deprecated

Instance Method

# sendMessage(withLocalizedFormatKey:arguments:data:to:badgePlayers:completionHandler:)

Sends a message to players in a game session.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func sendMessage(
    withLocalizedFormatKey key: String,
    arguments: [String],
    data: Data?,
    to players: [GKCloudPlayer],
    badgePlayers: Bool,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func sendMessage(
    withLocalizedFormatKey key: String,
    arguments: [String],
    data: Data?,
    to players: [GKCloudPlayer],
    badgePlayers: Bool
) async throws
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`key`  

A localized string with format tokens.

`arguments`  

An array containing entries for the format tokens contained by the `key` parameter.

`data`  

A `Data` object containing a limited amount of developer determined game information.

`players`  

A `GKCloudPlayer` array containing the players to be messaged.

`badgePlayers`  

A `Boolean` indicating whether players are badged when the message is sent.

`completionHandler`  

A block that is called after the message has been sent.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is nil. See `GameKit Constants` for a list of error codes specific to GameKit.

## See Also

### Communicating Between Players

var badgedPlayers: [GKCloudPlayer]

An array containing all of the currently badged players.

Deprecated

func clearBadge(for: [GKCloudPlayer], completionHandler: ((any Error)?) -> Void)

Clears the badge from the designated players.

Deprecated

