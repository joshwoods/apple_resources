

- UIKit
- UIBarAppearance
-  shadowImage 

Instance Property

# shadowImage

The image to use for the bar’s shadow.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var shadowImage: UIImage? { get set }
```

## Discussion

UIKit uses this property and the shadowColor property to determine the shadow’s appearance. When this property is `nil`, the bar displays a default shadow tinted according to the value in the shadowColor property. If shadowColor is `nil` or contains the clear color, the bar displays no shadow.

If this property contains a template image, the bar uses the image for the shadow and tints it using the value in shadowColor. If shadowColor is `nil` or contains the clear color, the bar displays no shadow. However, if this property doesn’t contain a template image, the bar displays the image without applying the shadow color.

## See Also

### Configuring the shadow appearance

var shadowColor: UIColor?

The color to apply to the bar’s custom or default shadow.

