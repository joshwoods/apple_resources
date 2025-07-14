

- UIKit
- UIBarAppearance
-  backgroundColor 

Instance Property

# backgroundColor

The background color of the bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var backgroundColor: UIColor? { get set }
```

## Discussion

The bar layers the specified color on top of any blur effects you specified in the backgroundEffect property, and below the image in the backgroundImage property.

## See Also

### Configuring the background appearance

var backgroundEffect: UIBlurEffect?

The blur effect to apply to the bar’s background.

var backgroundImage: UIImage?

The image to display on top of the bar’s background color.

var backgroundImageContentMode: UIView.ContentMode

The content mode to use when displaying the bar’s background image.

