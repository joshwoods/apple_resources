

- PDFKit
- PDFView
-  currentPage 

Instance Property

# currentPage

Returns the current page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
var currentPage: PDFPage? { get }
```

## Discussion

When there are two pages in the view in a two-up mode, “current page” is the left page. For continuous modes, returns the page crossing a horizontal line halfway between the view’s top and bottom bounds.

## See Also

### Related Documentation

func go(to: PDFDestination)

Navigates to the specified destination.

### Navigating Within a Document

var currentDestination: PDFDestination?

Returns a `PDFDestination` object representing the current page and the current point in the view specified in page space.

var visiblePages: [PDFPage]

Returns an array of `PDFPage` objects that represent the currently visible pages.

Navigation

Operations for moving through page history and seeking to a page in a document.

