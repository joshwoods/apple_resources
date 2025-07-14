

- GameKit
- GKGameSession
-  setConnectionState(\_:completionHandler:) Deprecated

Instance Method

# setConnectionState(\_:completionHandler:)

Sets the connection state for the player.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func setConnectionState(
    _ state: GKConnectionState,
    completionHandler: @escaping ((any Error)?) -> Void
)
```

``` source
func setConnectionState(_ state: GKConnectionState) async throws
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`state`  

The `GKConnectionState` to be assigned to the player.

`completionHandler`  

A block that is called after the connect state has been set.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is nil. See `GameKit Constants` for a list of error codes specific to GameKit.

## Discussion

This method will fail when the game session’s player limit has already been reached or there are network problems. The game session’s `lastModifiedDate` and `lastModifiedPlayer` properties are updated on completion.

## See Also

### Connecting Players for Real-Time Communication

func players(with: GKConnectionState) -> [GKCloudPlayer]

Retrieves a list of players with the specified connection state.

Deprecated

func send(Data, with: GKTransportType, completionHandler: ((any Error)?) -> Void)

Sends the indicated data to all connected players.

Deprecated

enum GKTransportType

The mechanism used to send messages to other players in a game session.

