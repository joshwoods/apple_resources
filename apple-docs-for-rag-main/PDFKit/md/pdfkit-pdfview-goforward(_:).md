

- PDFKit
- PDFView
-  goForward(\_:) 

Instance Method

# goForward(\_:)

Navigates forward one step in the page history.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@IBAction @MainActor
func goForward(_ sender: Any?)
```

## Discussion

The page history gets built as your application calls navigation methods such as go(to:) and goToLastPage(_:).

## See Also

### Related Documentation

var canGoForward: Bool

Returns a Boolean value indicating whether the user can navigate to the next page in the page history.

### Navigating History for a Document

func goBack(Any?)

Navigates back one step in the page history.

func goToFirstPage(Any?)

Navigates to the first page of the document.

func goToLastPage(Any?)

Navigates to the last page of the document.

func goToNextPage(Any?)

Navigates to the next page of the document.

func goToPreviousPage(Any?)

Navigates to the previous page of the document.

