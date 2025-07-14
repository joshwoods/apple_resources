

- UIKit
- UIPageControl
-  pageIndicatorTintColor 

Instance Property

# pageIndicatorTintColor

The tint color to apply to the page indicator.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var pageIndicatorTintColor: UIColor? { get set }
```

## Discussion

The default color is a translucent white for the page indicator dot. The page indicator dot is used for all of the pages not visible on the screen. Assigning a new value to this property does not automatically change the color in the currentPageIndicatorTintColor property because the value for these two properties is not automatically derived from the other. Both properties must be specified independently. Similarly, no alpha is applied to this property for you. It is recommended (but not required) that the color you specify for this parameter contains some transparency–i.e. the alpha value should be less than 1.0.

## See Also

### Coloring the page indicator

var currentPageIndicatorTintColor: UIColor?

The tint color to apply to the current page indicator.

