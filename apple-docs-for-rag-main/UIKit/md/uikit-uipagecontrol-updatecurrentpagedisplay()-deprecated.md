

- UIKit
- UIPageControl
-  updateCurrentPageDisplay() Deprecated

Instance Method

# updateCurrentPageDisplay()

Updates the page indicator to the current page.

iOS 2.0–14.0DeprecatediPadOS 2.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
func updateCurrentPageDisplay()
```

## Discussion

This method updates the page indicator so that the current page (the white dot) matches the value returned from currentPage. The class ignores this method if the value of defersCurrentPageDisplay is false. Setting the currentPage value directly updates the indicator immediately.

## See Also

### Managing pages

var currentPage: Int

The current page, shown by the page control as a white dot.

var numberOfPages: Int

The number of pages the receiver shows (as dots).

var hidesForSinglePage: Bool

A Boolean value that controls whether the page control is hidden when there is only one page.

var defersCurrentPageDisplay: Bool

A Boolean value that controls when the current page is displayed.

Deprecated

