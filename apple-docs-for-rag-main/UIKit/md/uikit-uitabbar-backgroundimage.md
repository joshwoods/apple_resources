

- UIKit
- UITabBar
-  backgroundImage 

Instance Property

# backgroundImage

The custom background image for the tab bar.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var backgroundImage: UIImage? { get set }
```

## Discussion

If you specify a stretchable background image, the tab bar stretches your image to fill the available space. If your image is not stretchable and not large enough to fill the available space, the tab bar tiles the image. For information about how stretching works, see the UIImage.ResizingMode type in UIImage.

When a custom background image is present, the tab bar does not draw any blur effects behind itself, even when the isTranslucent property is true.

## See Also

### Changing the background

var barTintColor: UIColor?

The tint color to apply to the tab bar background.

