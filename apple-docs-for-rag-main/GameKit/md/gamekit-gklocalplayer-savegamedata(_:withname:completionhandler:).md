

- GameKit
- GKLocalPlayer
-  saveGameData(\_:withName:completionHandler:) 

Instance Method

# saveGameData(\_:withName:completionHandler:)

Saves game data with the specified name.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
func saveGameData(
    _ data: Data,
    withName name: String,
    completionHandler handler: ((GKSavedGame?, (any Error)?) -> Void)? = nil
)
```

``` source
func saveGameData(
    _ data: Data,
    withName name: String
) async throws -> GKSavedGame
```

## Parameters 

`data`  

An object that contains the saved game data.

`name`  

A unique filename for the saved game data.

`handler`  

The block that this method calls when it completes the request.

The block receives the following parameters:

savedGame  
The saved game.

error  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Saving the player’s game data to an iCloud account

## Discussion

If the `name` parameter is an existing filename, GameKit overwrites the file with the new game data.

Important

You must provide an iCloud container ID in your project to save game data to the player’s iCloud account. Add the iCloud Container Identifiers Entitlement key to your project containing a unique identifier for your game.

## See Also

### Saving Game Data

Saving the player’s game data to an iCloud account

Save game data during play or after a game in the player’s iCloud account that’s accessible from any device.

func fetchSavedGames(completionHandler: (([GKSavedGame]?, (any Error)?) -> Void)?)

Retrieves all available saved games.

func resolveConflictingSavedGames([GKSavedGame], with: Data, completionHandler: (([GKSavedGame]?, (any Error)?) -> Void)?)

Replaces duplicate saved games that use the same filename with one file containing the specified game data.

func deleteSavedGames(withName: String, completionHandler: (((any Error)?) -> Void)?)

Deletes saved games with the specified filename.

class GKSavedGame

An object that represents a file containing saved game data.

protocol GKSavedGameListener

A protocol that handles events related to saving game data.

