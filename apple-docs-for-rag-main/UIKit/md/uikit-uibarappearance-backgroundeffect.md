

- UIKit
- UIBarAppearance
-  backgroundEffect 

Instance Property

# backgroundEffect

The blur effect to apply to the bar’s background.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var backgroundEffect: UIBlurEffect? { get set }
```

## Discussion

The blur effect provides the base layer for the bar’s appearance, and it determines how much of the underlying content is visible. UIKit applies the backgroundColor and backgroundImage on top of this effect.

## See Also

### Configuring the background appearance

var backgroundColor: UIColor?

The background color of the bar.

var backgroundImage: UIImage?

The image to display on top of the bar’s background color.

var backgroundImageContentMode: UIView.ContentMode

The content mode to use when displaying the bar’s background image.

