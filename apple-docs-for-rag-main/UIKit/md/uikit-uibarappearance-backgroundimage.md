

- UIKit
- UIBarAppearance
-  backgroundImage 

Instance Property

# backgroundImage

The image to display on top of the bar’s background color.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var backgroundImage: UIImage? { get set }
```

## Discussion

The bar layers the specified image on top of the content in the backgroundEffect and backgroundColor properties. UIKit sizes the image according to the value in the backgroundImageContentMode property.

## See Also

### Configuring the background appearance

var backgroundEffect: UIBlurEffect?

The blur effect to apply to the bar’s background.

var backgroundColor: UIColor?

The background color of the bar.

var backgroundImageContentMode: UIView.ContentMode

The content mode to use when displaying the bar’s background image.

