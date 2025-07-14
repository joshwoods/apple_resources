

- PDFKit
- PDFView
-  canGoBack 

Instance Property

# canGoBack

Returns a Boolean value indicating whether the user can navigate to the previous page in the page history.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var canGoBack: Bool { get }
```

## Discussion

The page history gets built as your application calls navigation methods such as go(to:) and goToLastPage(_:).

## See Also

### Related Documentation

func goBack(Any?)

Navigates back one step in the page history.

### Determining Valid History Operations

var canGoForward: Bool

Returns a Boolean value indicating whether the user can navigate to the next page in the page history.

var canGoToFirstPage: Bool

Returns a Boolean value indicating whether the user can navigate to the first page of the document.

var canGoToLastPage: Bool

Returns a Boolean value indicating whether the user can navigate to the last page of the document.

var canGoToNextPage: Bool

Returns a Boolean value indicating whether the user can navigate to the next page of the document.

var canGoToPreviousPage: Bool

Returns a Boolean value indicating whether the user can navigate to the previous page of the document.

