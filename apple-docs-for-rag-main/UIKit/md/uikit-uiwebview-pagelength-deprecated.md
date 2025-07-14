

- UIKit
- UIWebView
-  pageLength Deprecated

Instance Property

# pageLength

The size of each page, in points, in the direction that the pages flow.

iOS 7.0–12.0DeprecatediPadOS 7.0–12.0Deprecated

``` source
@MainActor
var pageLength: CGFloat { get set }
```

## Discussion

When paginationMode is right to left or left to right, this property represents the width of each page. When paginationMode is top to bottom or bottom to top, this property represents the height of each page.

The default value is `0`, which means the layout uses the size of the viewport to determine the dimensions of the page. Adjusting the value of this property causes a relayout.

## See Also

### Managing pages

var gapBetweenPages: CGFloat

The size of the gap, in points, between pages.

Deprecated

var pageCount: Int

The number of pages produced by the layout of the web view.

Deprecated

var paginationBreakingMode: UIWebView.PaginationBreakingMode

The manner in which column- or page-breaking occurs.

Deprecated

var paginationMode: UIWebView.PaginationMode

The layout of content in the web view.

Deprecated

