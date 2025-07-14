

- UIKit
- UIPageControl
-  preferredCurrentPageIndicatorImage 

Instance Property

# preferredCurrentPageIndicatorImage

The preferred image for the current page indicator.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
var preferredCurrentPageIndicatorImage: UIImage? { get set }
```

## Discussion

When `nil`, the page control uses preferredIndicatorImage as its current page indicator.

The default value of this property is `nil`.

## See Also

### Managing the indicator images

var preferredIndicatorImage: UIImage?

The preferred image for indicators.

func indicatorImage(forPage: Int) -> UIImage?

Returns the override image for the indicator of the specified page.

func setIndicatorImage(UIImage?, forPage: Int)

Registers an override image for the indicator of the specified page.

func currentPageIndicatorImage(forPage: Int) -> UIImage?

Returns the override image for the current page indicator of the specified page.

func setCurrentPageIndicatorImage(UIImage?, forPage: Int)

Registers an override image for the current page indicator of the specified page.

