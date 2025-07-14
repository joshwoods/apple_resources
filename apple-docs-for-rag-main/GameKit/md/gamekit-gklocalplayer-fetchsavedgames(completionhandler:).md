

- GameKit
- GKLocalPlayer
-  fetchSavedGames(completionHandler:) 

Instance Method

# fetchSavedGames(completionHandler:)

Retrieves all available saved games.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
func fetchSavedGames(completionHandler handler: (([GKSavedGame]?, (any Error)?) -> Void)? = nil)
```

``` source
func fetchSavedGames() async throws -> [GKSavedGame]
```

## Parameters 

`handler`  

The block that this method calls when it completes the request.

The block receives the following parameters:

savedGames  
An array of saved games that GameKit fetches.

error  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Saving the player’s game data to an iCloud account

## Discussion

If more than one saved game has the same filename, a conflict occurs and you must choose which saved game filename is correct using the resolveConflictingSavedGames(_:with:completionHandler:) method.

## See Also

### Saving Game Data

Saving the player’s game data to an iCloud account

Save game data during play or after a game in the player’s iCloud account that’s accessible from any device.

func saveGameData(Data, withName: String, completionHandler: ((GKSavedGame?, (any Error)?) -> Void)?)

Saves game data with the specified name.

func resolveConflictingSavedGames([GKSavedGame], with: Data, completionHandler: (([GKSavedGame]?, (any Error)?) -> Void)?)

Replaces duplicate saved games that use the same filename with one file containing the specified game data.

func deleteSavedGames(withName: String, completionHandler: (((any Error)?) -> Void)?)

Deletes saved games with the specified filename.

class GKSavedGame

An object that represents a file containing saved game data.

protocol GKSavedGameListener

A protocol that handles events related to saving game data.

