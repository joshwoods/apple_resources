

- UIKit
- UINavigationBarAppearance
-  setBackIndicatorImage(\_:transitionMaskImage:) 

Instance Method

# setBackIndicatorImage(\_:transitionMaskImage:)

Sets the back button indicator image and its transition mask.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func setBackIndicatorImage(
    _ backIndicatorImage: UIImage?,
    transitionMaskImage backIndicatorTransitionMaskImage: UIImage?
)
```

## Parameters 

`backIndicatorImage`  

The image to display on the leading edge of the back button.

`backIndicatorTransitionMaskImage`  

The image for masking content flowing under the back indicator image during push and pop transitions.

## Discussion

If you specify `nil` for either backIndicatorImage or backIndicatorTransitionMaskImage, this method resets both images to their default values.

## See Also

### Configuring the Back button

var backButtonAppearance: UIBarButtonItemAppearance

The appearance attributes for the back button.

var backIndicatorImage: UIImage

The image to display on the leading edge of the back button.

var backIndicatorTransitionMaskImage: UIImage

The image for masking content flowing under the back indicator image during push and pop transitions.

