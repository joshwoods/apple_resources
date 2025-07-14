

- PDFKit
- PDFView
-  Navigation 

API Collection

# Navigation

Operations for moving through page history and seeking to a page in a document.

## Topics

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

func goToPreviousPage(Any?)

Navigates to the previous page of the document.

### Using Seek in a Document

func go(to: PDFPage)

Scrolls to the specified page.

func go(to: PDFDestination)

Navigates to the specified destination.

func go(to: PDFSelection)

Scrolls to the first character of the specified selection.

func go(to: CGRect, on: PDFPage)

Navigates to the specified rectangle on the specified page.

## See Also

### Navigating Within a Document

var currentPage: PDFPage?

Returns the current page.

var currentDestination: PDFDestination?

Returns a `PDFDestination` object representing the current page and the current point in the view specified in page space.

var visiblePages: [PDFPage]

Returns an array of `PDFPage` objects that represent the currently visible pages.

