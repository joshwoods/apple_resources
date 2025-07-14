

- UIKit
- UIPageControl
-  currentPage 

Instance Property

# currentPage

The current page, shown by the page control as a white dot.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var currentPage: Int { get set }
```

## Discussion

The property value is an integer specifying the current page shown minus one; thus a value of zero (the default) indicates the first page. A page control shows the current page as a white dot. Values outside the possible range are pinned to either 0 or numberOfPages minus 1.

## See Also

### Managing pages

var numberOfPages: Int

The number of pages the receiver shows (as dots).

var hidesForSinglePage: Bool

A Boolean value that controls whether the page control is hidden when there is only one page.

var defersCurrentPageDisplay: Bool

A Boolean value that controls when the current page is displayed.

Deprecated

func updateCurrentPageDisplay()

Updates the page indicator to the current page.

Deprecated

