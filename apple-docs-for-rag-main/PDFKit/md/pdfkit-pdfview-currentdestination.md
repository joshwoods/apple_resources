

- PDFKit
- PDFView
-  currentDestination 

Instance Property

# currentDestination

Returns a `PDFDestination` object representing the current page and the current point in the view specified in page space.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var currentDestination: PDFDestination? { get }
```

## Discussion

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Related Documentation

func go(to: PDFDestination)

Navigates to the specified destination.

### Navigating Within a Document

var currentPage: PDFPage?

Returns the current page.

var visiblePages: [PDFPage]

Returns an array of `PDFPage` objects that represent the currently visible pages.

Navigation

Operations for moving through page history and seeking to a page in a document.

