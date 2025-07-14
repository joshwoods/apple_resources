

- UIKit
- UIToolbar
-  barTintColor 

Instance Property

# barTintColor

The tint color to apply to the toolbar background.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var barTintColor: UIColor? { get set }
```

## Discussion

This color is made translucent by default unless you set the isTranslucent property to false.

## See Also

### Changing the background

func backgroundImage(forToolbarPosition: UIBarPosition, barMetrics: UIBarMetrics) -> UIImage?

Returns the image to use for the background in a given position and with given metrics.

func setBackgroundImage(UIImage?, forToolbarPosition: UIBarPosition, barMetrics: UIBarMetrics)

Sets the image to use for the background in a given position and with given metrics.

