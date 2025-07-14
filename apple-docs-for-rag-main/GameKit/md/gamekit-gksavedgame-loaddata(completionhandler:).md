

- GameKit
- GKSavedGame
-  loadData(completionHandler:) 

Instance Method

# loadData(completionHandler:)

Loads the game data from the file.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
func loadData(completionHandler handler: ((Data?, (any Error)?) -> Void)? = nil)
```

``` source
func loadData() async throws -> Data
```

## Parameters 

`handler`  

The block that this method calls when it completes the request.

The block receives the following parameters:

*data*  
The data object that you saved to the file using the saveGameData(_:withName:completionHandler:) method

*error*  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Saving the player’s game data to an iCloud account

