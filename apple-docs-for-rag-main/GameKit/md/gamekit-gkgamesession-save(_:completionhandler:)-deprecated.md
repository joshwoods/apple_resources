

- GameKit
- GKGameSession
-  save(\_:completionHandler:) Deprecated

Instance Method

# save(\_:completionHandler:)

Saves the current game session data.

iOS 10.0–12.0DeprecatediPadOS 10.0–12.0DeprecatedMac Catalyst 13.1–13.1DeprecatedmacOS 10.12–10.14DeprecatedtvOS 10.0–12.0DeprecatedvisionOS 1.0–1.0Deprecated

``` source
func save(
    _ data: Data,
    completionHandler: @escaping (Data?, (any Error)?) -> Void
)
```

Deprecated

For real-time matches, use GKMatchmakerViewController. For turn-based matches, use GKTurnBasedMatchmakerViewController.

## Parameters 

`data`  

A `Data` object containing the information to be saved.

`completionHandler`  

A block that is called after the data has been saved.

data  
A `Data` object containing the information that is currently saved on the server.

error  
If an error occurred, this parameter holds an error object that explains the error. Otherwise, the value of this parameter is nil. See `GameKit Constants` for a list of error codes specific to GameKit.

## Discussion

The maximum amount of data to be saved is 512K. The `lastModifiedDate` and `lastModifiedPlayer` properties are updated upon completion. When a save conflict appears, the data is not saved to the server. The data property in the completion handler contains the information currently saved to the server. It is up to the developer to decide how to handle save conflicts.

## See Also

### Saving and Loading Data

func loadData(completionHandler: (Data?, (any Error)?) -> Void)

Retrieves the game data from the current game session.

Deprecated

