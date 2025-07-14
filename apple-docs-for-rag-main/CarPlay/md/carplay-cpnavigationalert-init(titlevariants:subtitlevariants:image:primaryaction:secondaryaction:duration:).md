

- CarPlay
- CPNavigationAlert
-  init(titleVariants:subtitleVariants:image:primaryAction:secondaryAction:duration:) 

Initializer

# init(titleVariants:subtitleVariants:image:primaryAction:secondaryAction:duration:)

Creates a navigation alert.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
init(
    titleVariants: [String],
    subtitleVariants: [String]?,
    image: UIImage?,
    primaryAction: CPAlertAction,
    secondaryAction: CPAlertAction?,
    duration: TimeInterval
)
```

## Parameters 

`titleVariants`  

An array of localized, displayable titles in order of preference. CarPlay displays the title that fits in the available screen space.

`subtitleVariants`  

An array of localized, displayable subtitles in order of preference. CarPlay displays the subtitle that fits in the available screen space.

`image`  

The image the alert displays.

`primaryAction`  

The alert’s primary action.

`secondaryAction`  

The alert’s secondary action.

`duration`  

The amount of time, in seconds, that the alert remains visible. If you provide a duration of 0, CarPlay displays the alert until the user dismisses it.

## Discussion

Provide an image that is display-ready. If necessary, provide light and dark variants using an asset catalog, or use an instance of UIImageAsset and register an image for each interface style. To properly size your image, use the display scale of the vehicle’s primary screen, which you access from your interface controller’s carTraitCollection property.

CarPlay doesn’t support animated images. If you provide an animated image, CarPlay uses only the first image in the animation sequence.

## See Also

### Creating a Navigation Alert

init(titleVariants: [String], subtitleVariants: [String]?, imageSet: CPImageSet?, primaryAction: CPAlertAction, secondaryAction: CPAlertAction?, duration: TimeInterval)

Creates a navigation alert.

Deprecated

