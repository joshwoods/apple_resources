

- GameKit
- GKGameSession
-  send(\_:with:completionHandler:) Deprecated

Instance Method

# send(\_:with:completionHandler:)

Sends the indicated data to all connected players.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func send(
    _ data: Data,
    with transport: GKTransportType,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func send(
    _ data: Data,
    with transport: GKTransportType
) async throws
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`data`  

A `Data` object containing the information to be sent.

`transport`  

Determines how the data is sent.

`completionHandler`  

A block that is called after the data has been sent.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is nil. See `GameKit Constants` for a list of error codes specific to GameKit.

## See Also

### Connecting Players for Real-Time Communication

func setConnectionState(GKConnectionState, completionHandler: ((any Error)?) -> Void)

Sets the connection state for the player.

Deprecated

func players(with: GKConnectionState) -> [GKCloudPlayer]

Retrieves a list of players with the specified connection state.

Deprecated

enum GKTransportType

The mechanism used to send messages to other players in a game session.

