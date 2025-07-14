

- UIKit
- UITabBarAppearance
-  selectionIndicatorTintColor 

Instance Property

# selectionIndicatorTintColor

The tint color to apply to the selection indicator image.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var selectionIndicatorTintColor: UIColor? { get set }
```

## Discussion

UIKit combines the color in this property with the image in the selectionIndicatorImage to create the final appearance for the selected item. If you supplied a template image in selectionIndicatorImage, UIKit uses this color to tint that image. If selectionIndicatorImage is `nil`, UIKit provides a default selection indicator image that accepts your tint color. If this property is `nil` or contains a clear color, UIKit doesn’t display a selection indicator.

If the image you supplied in selectionIndicatorImage isn’t a template image, UIKit ignores the value in this property and displays your image as is.

The default value of this property is `nil`.

## See Also

### Specifying the selection appearance

var selectionIndicatorImage: UIImage?

The image to draw for the selected item.

