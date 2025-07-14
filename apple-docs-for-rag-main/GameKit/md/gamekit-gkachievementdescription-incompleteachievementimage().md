

- GameKit
- GKAchievementDescription
-  incompleteAchievementImage() 

Type Method

# incompleteAchievementImage()

A common image that you can display when the player hasn’t completed the achievement.

iOSiPadOSMac CatalystmacOStvOSvisionOS

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
class func incompleteAchievementImage() -> UIImage
```

**macOS**

``` source
class func incompleteAchievementImage() -> NSImage
```

## Return Value

A common image that represents an incomplete achievement.

## Discussion

In macOS versions earlier than macOS 11, this class method returns an NSImage object but otherwise works the same as in iOS, Mac Catalyst, and tvOS.

Starting with iOS 14, macOS 11, and tvOS 14, this method returns a symbol image. To match your game’s appearance, make adjustments to the symbol image as described in Configuring and displaying symbol images in your UI.

## See Also

### Working with Achievement Images

class func placeholderCompletedAchievementImage() -> UIImage

A placeholder image that you can display when the player completes the achievement.

func loadImage(completionHandler: ((UIImage?, (any Error)?) -> Void)?)

Loads the image to display when the player completes the achievement.

