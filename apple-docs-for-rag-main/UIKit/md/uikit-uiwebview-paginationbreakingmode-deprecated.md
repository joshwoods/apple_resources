

- UIKit
- UIWebView
-  paginationBreakingMode Deprecated

Instance Property

# paginationBreakingMode

The manner in which column- or page-breaking occurs.

iOS 7.0–12.0DeprecatediPadOS 7.0–12.0Deprecated

``` source
@MainActor
var paginationBreakingMode: UIWebView.PaginationBreakingMode { get set }
```

## Discussion

This property determines whether certain CSS properties regarding column- and page-breaking are honored or ignored. When this property is set to UIWebView.PaginationBreakingMode.column, the content respects the CSS properties related to column-breaking in place of page-breaking.

See UIWebView.PaginationBreakingMode for possible values. The default value is UIWebView.PaginationBreakingMode.page.

## See Also

### Managing pages

var gapBetweenPages: CGFloat

The size of the gap, in points, between pages.

Deprecated

var pageCount: Int

The number of pages produced by the layout of the web view.

Deprecated

var pageLength: CGFloat

The size of each page, in points, in the direction that the pages flow.

Deprecated

var paginationMode: UIWebView.PaginationMode

The layout of content in the web view.

Deprecated

