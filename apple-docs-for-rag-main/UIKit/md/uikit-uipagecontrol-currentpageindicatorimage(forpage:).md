

- UIKit
- UIPageControl
-  currentPageIndicatorImage(forPage:) 

Instance Method

# currentPageIndicatorImage(forPage:)

Returns the override image for the current page indicator of the specified page.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+tvOS 16.0+visionOS 1.0+

``` source
@MainActor
func currentPageIndicatorImage(forPage page: Int) -> UIImage?
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

func indicatorImage(forPage: Int) -> UIImage?

Returns the override image for the indicator of the specified page.

func setIndicatorImage(UIImage?, forPage: Int)

Registers an override image for the indicator of the specified page.

var preferredCurrentPageIndicatorImage: UIImage?

The preferred image for the current page indicator.

func setCurrentPageIndicatorImage(UIImage?, forPage: Int)

Registers an override image for the current page indicator of the specified page.

