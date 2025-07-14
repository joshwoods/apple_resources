

- UIKit
- UIBarAppearance
-  shadowColor 

Instance Property

# shadowColor

The color to apply to the bar’s custom or default shadow.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var shadowColor: UIColor? { get set }
```

## Discussion

UIKit uses this property and the shadowImage property to determine the shadow’s appearance. When shadowImage is `nil`, the bar displays a default shadow tinted according to the value of this property. If this property is `nil` or contains the clear color, the bar displays no shadow.

If shadowImage contains a template image, the bar uses the image for the shadow and tints it using the value in this property. If this property is `nil` or contains the clear color, the bar displays no shadow. However, if shadowImage doesn’t contain a template image, the bar displays the image without applying the color in this property.

## See Also

### Configuring the shadow appearance

var shadowImage: UIImage?

The image to use for the bar’s shadow.

