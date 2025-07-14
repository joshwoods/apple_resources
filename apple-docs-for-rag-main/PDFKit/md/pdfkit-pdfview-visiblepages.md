

- PDFKit
- PDFView
-  visiblePages 

Instance Property

# visiblePages

Returns an array of `PDFPage` objects that represent the currently visible pages.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.5+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var visiblePages: [PDFPage] { get }
```

## See Also

### Navigating Within a Document

var currentPage: PDFPage?

Returns the current page.

var currentDestination: PDFDestination?

Returns a `PDFDestination` object representing the current page and the current point in the view specified in page space.

Navigation

Operations for moving through page history and seeking to a page in a document.

