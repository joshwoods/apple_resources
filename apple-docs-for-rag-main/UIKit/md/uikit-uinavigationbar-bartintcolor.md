

- UIKit
- UINavigationBar
-  barTintColor 

Instance Property

# barTintColor

The tint color to apply to the navigation bar background.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var barTintColor: UIColor? { get set }
```

## Discussion

This color is made translucent by default unless you set the isTranslucent property to false.

## See Also

### Changing the background

func backgroundImage(for: UIBarMetrics) -> UIImage?

Returns the background image for given bar metrics.

func setBackgroundImage(UIImage?, for: UIBarMetrics)

Sets the background image for given bar metrics.

func backgroundImage(for: UIBarPosition, barMetrics: UIBarMetrics) -> UIImage?

Returns the background image to use for a given bar position and set of metrics.

func setBackgroundImage(UIImage?, for: UIBarPosition, barMetrics: UIBarMetrics)

Sets the background image to use for a given bar position and set of metrics.

