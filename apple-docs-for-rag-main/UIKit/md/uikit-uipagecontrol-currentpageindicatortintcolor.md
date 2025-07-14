

- UIKit
- UIPageControl
-  currentPageIndicatorTintColor 

Instance Property

# currentPageIndicatorTintColor

The tint color to apply to the current page indicator.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var currentPageIndicatorTintColor: UIColor? { get set }
```

## Discussion

The default color is an opaque white for the current page indicator dot. The current page indicator dot is used to indicate the currently visible page. Assigning a new value to this property does not automatically change the color in the pageIndicatorTintColor property because the value for these two properties is not automatically derived from the other. Both properties must be specified independently.

## See Also

### Coloring the page indicator

var pageIndicatorTintColor: UIColor?

The tint color to apply to the page indicator.

