

- GameKit
-  GKSavedGame 

Class

# GKSavedGame

An object that represents a file containing saved game data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
class GKSavedGame
```

## Mentioned in 

Saving the player’s game data to an iCloud account

## Overview

A `GKSavedGame` object represents the file that contains game data you saved using the `GKLocalPlayer` saveGameData(_:withName:completionHandler:) method.

You don’t create `GKSavedGame` objects directly. Instead use the fetchSavedGames(completionHandler:) method to get the games you saved. Then get the filename, its modification date, and the name of the device the player used to save the game from the returned objects.

Use the loadData(completionHandler:) method to get the actual game data you saved in the file. To delete saved games, use the deleteSavedGames(withName:completionHandler:) method.

## Topics

### Loading Saved Game Data

func loadData(completionHandler: ((Data?, (any Error)?) -> Void)?)

Loads the game data from the file.

### Retrieving Information About a Saved Game File

var name: String?

The name of the saved game.

var modificationDate: Date?

The date when you saved the game data or modified it.

var deviceName: String?

The name of the device that the player uses to save the game.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

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

func deleteSavedGames(withName: String, completionHandler: (((any Error)?) -> Void)?)

Deletes saved games with the specified filename.

protocol GKSavedGameListener

A protocol that handles events related to saving game data.

