

- GameKit
- GKGameSession
-  title Deprecated

Instance Property

# title

The title of the game session.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
var title: String { get }
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## See Also

### Accessing Information About a Game Session

var identifier: String

A unique identifier for a game session.

Deprecated

var lastModifiedDate: Date

The date that the game session was last modified.

Deprecated

var lastModifiedPlayer: GKCloudPlayer

The last player to modify the game session.

Deprecated

var maxNumberOfConnectedPlayers: Int

The maximum number of players allowed to connect to the game session at the same time.

Deprecated

var owner: GKCloudPlayer

A player object that represents the owner of the game session.

Deprecated

var players: [GKCloudPlayer]

An array of player objects associated with the game session.

Deprecated

