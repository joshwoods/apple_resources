

- UIKit
- UITabBarItem
-  selectedImage 

Instance Property

# selectedImage

The source image the item uses to generate its selected image.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var selectedImage: UIImage? { get set }
```

## Discussion

If `nil`, the item uses the value in image instead. The item creates the images it displays from the alpha values in its source images. To prevent system tinting, use images with the UIImage.RenderingMode.alwaysOriginal rendering mode. The item clips any image that’s larger than its bounds.

## See Also

### Configuring the item’s appearance

var standardAppearance: UITabBarAppearance?

The appearance settings for a tab bar.

var scrollEdgeAppearance: UITabBarAppearance?

The appearance settings for the tab bar when the edge of scrollable content aligns with the edge of the tab bar.

var titlePositionAdjustment: UIOffset

The offset to apply to the title’s position.

