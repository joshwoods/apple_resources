

- PDFKit
- PDFView
-  go(to:on:) 

Instance Method

# go(to:on:)

Navigates to the specified rectangle on the specified page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**macOS**

``` source
@MainActor
func go(
    to rect: NSRect,
    on page: PDFPage
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
func go(
    to rect: CGRect,
    on page: PDFPage
)
```

## Discussion

If the specified rectangle is already visible, this method does nothing. This allows you to scroll the `PDFView` object to a specific PDFAnnotation or PDFSelection object, because both of these objects have bounds methods that return an annotation or selection position in page space.

Note that `rect` is specified in page-space coordinates. Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Using Seek in a Document

func go(to: PDFPage)

Scrolls to the specified page.

func go(to: PDFDestination)

Navigates to the specified destination.

func go(to: PDFSelection)

Scrolls to the first character of the specified selection.

