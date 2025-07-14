

- UIKit
- UIPageControl
-  hidesForSinglePage 

Instance Property

# hidesForSinglePage

A Boolean value that controls whether the page control is hidden when there is only one page.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var hidesForSinglePage: Bool { get set }
```

## Discussion

Assign a value of true to hide the page control when there is only one page; assign false (the default) to show the page control if there is only one page.

## See Also

### Managing pages

var currentPage: Int

The current page, shown by the page control as a white dot.

var numberOfPages: Int

The number of pages the receiver shows (as dots).

var defersCurrentPageDisplay: Bool

A Boolean value that controls when the current page is displayed.

Deprecated

func updateCurrentPageDisplay()

Updates the page indicator to the current page.

Deprecated

