

- UIKit
- UIPageControl
-  preferredIndicatorImage 

Instance Property

# preferredIndicatorImage

The preferred image for indicators.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
var preferredIndicatorImage: UIImage? { get set }
```

## See Also

### Managing the indicator images

func indicatorImage(forPage: Int) -> UIImage?

Returns the override image for the indicator of the specified page.

func setIndicatorImage(UIImage?, forPage: Int)

Registers an override image for the indicator of the specified page.

var preferredCurrentPageIndicatorImage: UIImage?

The preferred image for the current page indicator.

func currentPageIndicatorImage(forPage: Int) -> UIImage?

Returns the override image for the current page indicator of the specified page.

func setCurrentPageIndicatorImage(UIImage?, forPage: Int)

Registers an override image for the current page indicator of the specified page.

