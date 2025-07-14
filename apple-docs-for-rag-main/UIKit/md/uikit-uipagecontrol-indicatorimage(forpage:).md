

- UIKit
- UIPageControl
-  indicatorImage(forPage:) 

Instance Method

# indicatorImage(forPage:)

Returns the override image for the indicator of the specified page.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+

``` source
@MainActor
func indicatorImage(forPage page: Int) -> UIImage?
```

## Parameters 

`page`  

The index of the page. A value that’s greater than or equal to `0` and less than numberOfPages.

## Return Value

The override image, or `nil` if you haven’t overidden the image for the specified page number.

## See Also

### Managing the indicator images

var preferredIndicatorImage: UIImage?

The preferred image for indicators.

func setIndicatorImage(UIImage?, forPage: Int)

Registers an override image for the indicator of the specified page.

var preferredCurrentPageIndicatorImage: UIImage?

The preferred image for the current page indicator.

func currentPageIndicatorImage(forPage: Int) -> UIImage?

Returns the override image for the current page indicator of the specified page.

func setCurrentPageIndicatorImage(UIImage?, forPage: Int)

Registers an override image for the current page indicator of the specified page.

