

- GameKit
- GKAchievementDescription
-  loadImage(completionHandler:) 

Instance Method

# loadImage(completionHandler:)

Loads the image to display when the player completes the achievement.

iOSiPadOSMac CatalystmacOStvOSvisionOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func loadImage(completionHandler: ((UIImage?, (any Error)?) -> Void)? = nil)
```

**macOS**

``` source
func loadImage(completionHandler: ((NSImage?, (any Error)?) -> Void)? = nil)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
func loadImage() async throws -> UIImage
```

**macOS**

``` source
func loadImage() async throws -> NSImage
```

## Parameters 

`completionHandler`  

A block that GameKit calls when this method completes the download.

The block receives the following parameters:

`image`  
The image that represents the completed achievement. This parameter is `nil` if an error occurs.

`error`  
Describes an error if it occurs, or `nil` if the operation completes.

## Mentioned in 

Rewarding players with achievements

## Discussion

First, use the loadAchievementDescriptions(completionHandler:) method to download the achievement description objects, and then use this method to download the individual achievement images. While GameKit downloads an achievement image, you can display the placeholder image. If successful, GameKit sets the image property to the image it passes to the completion handler.

## See Also

### Working with Achievement Images

class func incompleteAchievementImage() -> UIImage

A common image that you can display when the player hasn’t completed the achievement.

class func placeholderCompletedAchievementImage() -> UIImage

A placeholder image that you can display when the player completes the achievement.

