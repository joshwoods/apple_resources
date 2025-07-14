

- GameKit
- GKSavedGameListener
-  player(\_:hasConflictingSavedGames:) 

Instance Method

# player(\_:hasConflictingSavedGames:)

Chooses the correct game data from the saved games that contain conflicts.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
optional func player(
    _ player: GKPlayer,
    hasConflictingSavedGames savedGames: [GKSavedGame]
)
```

## Parameters 

`player`  

The player who saves the game data.

`savedGames`  

The saved games that contain the conflicts.

## Mentioned in 

Saving the player’s game data to an iCloud account

## Discussion

Saved game files conflict when multiple devices write to the same file while one or more of the devices are offline. Implement this method to choose the game data that’s correct and try saving it again using the resolveConflictingSavedGames(_:with:completionHandler:) method.

