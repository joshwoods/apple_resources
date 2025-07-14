

- PDFKit
- PDFView
-  canGoToPreviousPage 

Instance Property

# canGoToPreviousPage

Returns a Boolean value indicating whether the user can navigate to the previous page of the document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var canGoToPreviousPage: Bool { get }
```

## Discussion

The return value will be true unless the view is displaying the first page.

## See Also

### Determining Valid History Operations

var canGoBack: Bool

Returns a Boolean value indicating whether the user can navigate to the previous page in the page history.

var canGoForward: Bool

Returns a Boolean value indicating whether the user can navigate to the next page in the page history.

var canGoToFirstPage: Bool

Returns a Boolean value indicating whether the user can navigate to the first page of the document.

var canGoToLastPage: Bool

Returns a Boolean value indicating whether the user can navigate to the last page of the document.

var canGoToNextPage: Bool

Returns a Boolean value indicating whether the user can navigate to the next page of the document.

