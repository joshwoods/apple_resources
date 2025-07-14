

- GameKit
- GKLocalPlayer
-  deleteSavedGames(withName:completionHandler:) 

Instance Method

# deleteSavedGames(withName:completionHandler:)

Deletes saved games with the specified filename.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
func deleteSavedGames(
    withName name: String,
    completionHandler handler: (((any Error)?) -> Void)? = nil
)
```

``` source
func deleteSavedGames(withName name: String) async throws
```

## Parameters 

`name`  

A string that identifies the saved game data to delete.

`handler`  

The block that this method calls when it completes the request.

The block receives the following parameters:

error  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Saving the player’s game data to an iCloud account

## Discussion

Alternatively, use the resolveConflictingSavedGames(_:with:completionHandler:) method to keep one of the saved games that use the same filename.

## See Also

### Saving Game Data

Saving the player’s game data to an iCloud account

Save game data during play or after a game in the player’s iCloud account that’s accessible from any device.

func saveGameData(Data, withName: String, completionHandler: ((GKSavedGame?, (any Error)?) -> Void)?)

Saves game data with the specified name.

func fetchSavedGames(completionHandler: (([GKSavedGame]?, (any Error)?) -> Void)?)

Retrieves all available saved games.

func resolveConflictingSavedGames([GKSavedGame], with: Data, completionHandler: (([GKSavedGame]?, (any Error)?) -> Void)?)

Replaces duplicate saved games that use the same filename with one file containing the specified game data.

class GKSavedGame

An object that represents a file containing saved game data.

protocol GKSavedGameListener

A protocol that handles events related to saving game data.

