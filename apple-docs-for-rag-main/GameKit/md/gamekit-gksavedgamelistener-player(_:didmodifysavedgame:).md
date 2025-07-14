

- GameKit
- GKSavedGameListener
-  player(\_:didModifySavedGame:) 

Instance Method

# player(\_:didModifySavedGame:)

Handles when data changes in a saved game file.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
optional func player(
    _ player: GKPlayer,
    didModifySavedGame savedGame: GKSavedGame
)
```

## Parameters 

`player`  

The player who saves the game data.

`savedGame`  

The game the player saves.

## Discussion

GameKit invokes this method when you save game data on a device that isn’t the user’s current device.

