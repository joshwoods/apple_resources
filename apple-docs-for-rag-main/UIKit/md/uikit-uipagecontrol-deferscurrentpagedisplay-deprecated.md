

- UIKit
- UIPageControl
-  defersCurrentPageDisplay Deprecated

Instance Property

# defersCurrentPageDisplay

A Boolean value that controls when the current page is displayed.

iOS 2.0–14.0DeprecatediPadOS 2.0–14.0DeprecatedMac Catalyst 13.1–14.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
@MainActor
var defersCurrentPageDisplay: Bool { get set }
```

## Discussion

Set the value of this property to true so that, when the user taps the control to go to a new page, the class defers updating the page control until it calls updateCurrentPageDisplay(). Set the value to false (the default) to have the page control updated immediately.

## See Also

### Managing pages

var currentPage: Int

The current page, shown by the page control as a white dot.

var numberOfPages: Int

The number of pages the receiver shows (as dots).

var hidesForSinglePage: Bool

A Boolean value that controls whether the page control is hidden when there is only one page.

func updateCurrentPageDisplay()

Updates the page indicator to the current page.

Deprecated

