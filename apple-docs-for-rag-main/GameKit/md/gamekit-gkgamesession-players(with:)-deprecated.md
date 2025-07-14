

- GameKit
- GKGameSession
-  players(with:) Deprecated

Instance Method

# players(with:)

Retrieves a list of players with the specified connection state.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func players(with state: GKConnectionState) -> [GKCloudPlayer]
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`state`  

A GKConnectionState used to find the requested players.

## Return Value

An array of players with the indicated connection state.

## See Also

### Connecting Players for Real-Time Communication

func setConnectionState(GKConnectionState, completionHandler: ((any Error)?) -> Void)

Sets the connection state for the player.

Deprecated

func send(Data, with: GKTransportType, completionHandler: ((any Error)?) -> Void)

Sends the indicated data to all connected players.

Deprecated

enum GKTransportType

The mechanism used to send messages to other players in a game session.

