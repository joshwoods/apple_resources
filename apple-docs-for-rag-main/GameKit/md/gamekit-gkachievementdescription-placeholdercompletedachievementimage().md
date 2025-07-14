

- GameKit
- GKAchievementDescription
-  placeholderCompletedAchievementImage() 

Type Method

# placeholderCompletedAchievementImage()

A placeholder image that you can display when the player completes the achievement.

iOSiPadOSMac CatalystmacOStvOSvisionOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
class func placeholderCompletedAchievementImage() -> UIImage
```

**macOS**

``` source
class func placeholderCompletedAchievementImage() -> NSImage
```

## Return Value

A common image that represents a completed achievement.

## Discussion

When the player completes the achievement, you can display this image as a placeholder until GameKit downloads the achievement’s image that you upload to App Store Connect.

In macOS versions earlier than macOS 11, this class method returns an NSImage object but otherwise works the same as in iOS, Mac Catalyst, and tvOS.

Starting with iOS 14, macOS 11, and tvOS 14, this method returns a symbol image. To match your game’s appearance, make adjustments to the symbol image as described in Configuring and displaying symbol images in your UI.

## See Also

### Working with Achievement Images

class func incompleteAchievementImage() -> UIImage

A common image that you can display when the player hasn’t completed the achievement.

func loadImage(completionHandler: ((UIImage?, (any Error)?) -> Void)?)

Loads the image to display when the player completes the achievement.

