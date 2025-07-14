

- UIKit
- UIWebView
-  paginationMode Deprecated

Instance Property

# paginationMode

The layout of content in the web view.

iOS 7.0–12.0DeprecatediPadOS 7.0–12.0Deprecated

``` source
@MainActor
var paginationMode: UIWebView.PaginationMode { get set }
```

## Discussion

This property determines whether content in the web view is broken up into pages that fill the view one screen at a time, or shown as one long scrolling view. If set to a paginated form, this property toggles a paginated layout on the content, causing the web view to use the values of pageLength and gapBetweenPages to relayout its content.

See UIWebView.PaginationMode for possible values. The default value is UIWebView.PaginationMode.unpaginated.

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

var paginationBreakingMode: UIWebView.PaginationBreakingMode

The manner in which column- or page-breaking occurs.

Deprecated

