

- GameKit
- GKGameSession
-  loadData(completionHandler:) Deprecated

Instance Method

# loadData(completionHandler:)

Retrieves the game data from the current game session.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func loadData(completionHandler: @escaping (Data?, (any Error)?) -> Void)
```

``` source
func loadData() async throws -> Data
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`completionHandler`  

A block that is called after the game session data has been loaded.

data  
A `Data` object containing the app’s saved data.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is nil. See `GameKit Constants` for a list of error codes specific to GameKit.

## See Also

### Saving and Loading Data

func save(Data, completionHandler: (Data?, (any Error)?) -> Void)

Saves the current game session data.

Deprecated

