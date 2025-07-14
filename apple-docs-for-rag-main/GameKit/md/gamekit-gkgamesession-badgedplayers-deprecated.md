

- GameKit
- GKGameSession
-  badgedPlayers Deprecated

Instance Property

# badgedPlayers

An array containing all of the currently badged players.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var badgedPlayers: [GKCloudPlayer] { get }
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## See Also

### Communicating Between Players

func clearBadge(for: [GKCloudPlayer], completionHandler: ((any Error)?) -> Void)

Clears the badge from the designated players.

Deprecated

func sendMessage(withLocalizedFormatKey: String, arguments: [String], data: Data?, to: [GKCloudPlayer], badgePlayers: Bool, completionHandler: ((any Error)?) -> Void)

Sends a message to players in a game session.

Deprecated

