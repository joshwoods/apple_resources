

- UIKit
- UIPageControl
-  numberOfPages 

Instance Property

# numberOfPages

The number of pages the receiver shows (as dots).

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var numberOfPages: Int { get set }
```

## Discussion

The value of the property is the number of pages for the page control to show as dots. The default value is 0.

## See Also

### Managing pages

var currentPage: Int

The current page, shown by the page control as a white dot.

var hidesForSinglePage: Bool

A Boolean value that controls whether the page control is hidden when there is only one page.

var defersCurrentPageDisplay: Bool

A Boolean value that controls when the current page is displayed.

Deprecated

func updateCurrentPageDisplay()

Updates the page indicator to the current page.

Deprecated

