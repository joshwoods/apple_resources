

- GameKit
- GKSavedGame
-  modificationDate 

Instance Property

# modificationDate

The date when you saved the game data or modified it.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+

``` source
var modificationDate: Date? { get }
```

## Discussion

Game Center sets this property when you save game data using the saveGameData(_:withName:completionHandler:) method. If you save game data using an existing filename, Game Center overwrites the file with the new data and changes the modification date.

## See Also

### Retrieving Information About a Saved Game File

var name: String?

The name of the saved game.

var deviceName: String?

The name of the device that the player uses to save the game.

