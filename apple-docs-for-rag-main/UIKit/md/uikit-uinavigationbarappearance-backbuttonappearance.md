

- UIKit
- UINavigationBarAppearance
-  backButtonAppearance 

Instance Property

# backButtonAppearance

The appearance attributes for the back button.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var backButtonAppearance: UIBarButtonItemAppearance { get set }
```

## Discussion

If you don’t change the value of this property, the navigation bar applies the attributes from the buttonAppearance property.

## See Also

### Configuring the Back button

var backIndicatorImage: UIImage

The image to display on the leading edge of the back button.

var backIndicatorTransitionMaskImage: UIImage

The image for masking content flowing under the back indicator image during push and pop transitions.

func setBackIndicatorImage(UIImage?, transitionMaskImage: UIImage?)

Sets the back button indicator image and its transition mask.

