

- CarPlay
- CPNavigationAlert
-  init(titleVariants:subtitleVariants:imageSet:primaryAction:secondaryAction:duration:) Deprecated

Initializer

# init(titleVariants:subtitleVariants:imageSet:primaryAction:secondaryAction:duration:)

Creates a navigation alert.

iOS 12.0–13.0DeprecatediPadOS 12.0–13.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
init(
    titleVariants: [String],
    subtitleVariants: [String]?,
    imageSet: CPImageSet?,
    primaryAction: CPAlertAction,
    secondaryAction: CPAlertAction?,
    duration: TimeInterval
)
```

## Parameters 

`titleVariants`  

An array of localized, displayable titles. The system selects the title that fits in the available display space.

`subtitleVariants`  

An array of localized, displayable subtitles. The system selects the title that fits in the available display space.

`imageSet`  

An image set displayed in the navigation alert. The navigation alert doesn’t support animated images. If you provide an animated image, the alert uses the first image in the animation sequence.

`primaryAction`  

The primary action and its button.

`secondaryAction`  

An optional, secondary action with its button.

`duration`  

The amount of time, in seconds, that the alert is visible. Setting the duration to 0 displays the alert until dismissed by the user.

## Return Value

A newly initialized navigation alert.

## See Also

### Creating a Navigation Alert

init(titleVariants: [String], subtitleVariants: [String]?, image: UIImage?, primaryAction: CPAlertAction, secondaryAction: CPAlertAction?, duration: TimeInterval)

Creates a navigation alert.

