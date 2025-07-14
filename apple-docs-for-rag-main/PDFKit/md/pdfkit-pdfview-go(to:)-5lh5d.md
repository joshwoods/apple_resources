

- PDFKit
- PDFView
-  go(to:) 

Instance Method

# go(to:)

Navigates to the specified destination.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func go(to destination: PDFDestination)
```

## Discussion

Destinations include a page and a point on the page specified in page space.

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Related Documentation

var currentPage: PDFPage?

Returns the current page.

var currentDestination: PDFDestination?

Returns a `PDFDestination` object representing the current page and the current point in the view specified in page space.

### Using Seek in a Document

func go(to: PDFPage)

Scrolls to the specified page.

func go(to: PDFSelection)

Scrolls to the first character of the specified selection.

func go(to: CGRect, on: PDFPage)

Navigates to the specified rectangle on the specified page.

