

- PDFKit
- PDFView
-  goToPreviousPage(\_:) 

Instance Method

# goToPreviousPage(\_:)

Navigates to the previous page of the document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@IBAction @MainActor
func goToPreviousPage(_ sender: Any?)
```

## Discussion

PDF Kit records the move in its page history.

## See Also

### Related Documentation

var canGoToPreviousPage: Bool

Returns a Boolean value indicating whether the user can navigate to the previous page of the document.

### Navigating History for a Document

func goBack(Any?)

Navigates back one step in the page history.

func goForward(Any?)

Navigates forward one step in the page history.

func goToFirstPage(Any?)

Navigates to the first page of the document.

func goToLastPage(Any?)

Navigates to the last page of the document.

func goToNextPage(Any?)

Navigates to the next page of the document.

