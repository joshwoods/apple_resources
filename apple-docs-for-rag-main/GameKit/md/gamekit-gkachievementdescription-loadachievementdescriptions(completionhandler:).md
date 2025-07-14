

- GameKit
- GKAchievementDescription
-  loadAchievementDescriptions(completionHandler:) 

Type Method

# loadAchievementDescriptions(completionHandler:)

Downloads the localized descriptions of achievements from Game Center.

iOS 4.1+iPadOS 4.1+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 3.0+

``` source
class func loadAchievementDescriptions(completionHandler: (([GKAchievementDescription]?, (any Error)?) -> Void)? = nil)
```

``` source
class func loadAchievementDescriptions() async throws -> [GKAchievementDescription]
```

## Parameters 

`completionHandler`  

A block that GameKit calls when this method completes the download.

The block receives the following parameters:

`descriptions`  
The GKAchievementDescription objects that contain the localized text for the achievements in your game.

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Rewarding players with achievements

## Discussion

To load the artwork for an achievement, use the loadImage(completionHandler:) method after using this method.

