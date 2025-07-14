

- GameKit
-  GKSavedGameListener 

Protocol

# GKSavedGameListener

A protocol that handles events related to saving game data.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
protocol GKSavedGameListener : NSObjectProtocol
```

## Overview

Implement the methods in the this protocol to manage conflicts or track changes when saving game data.

Adopt the GKLocalPlayerListener protocol to listen for and handle a variety of Game Center events for player accounts instead of the individual GKChallengeListener, GKInviteEventListener, GKSavedGameListener, and GKTurnBasedEventListener protocols.

## Topics

### Handling Saved Game Conflicts

func player(GKPlayer, hasConflictingSavedGames: [GKSavedGame])

Chooses the correct game data from the saved games that contain conflicts.

### Handling Saved Game Changes

func player(GKPlayer, didModifySavedGame: GKSavedGame)

Handles when data changes in a saved game file.

## Relationships

### Inherits From

- NSObjectProtocol

### Inherited By

- GKLocalPlayerListener

### Conforming Types

- GKLocalPlayer

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

class GKSavedGame

An object that represents a file containing saved game data.

