

- PDFKit
- PDFView
-  go(to:) 

Instance Method

# go(to:)

Scrolls to the specified page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func go(to page: PDFPage)
```

## Discussion

PDF Kit records the move in its page history.

## See Also

### Using Seek in a Document

func go(to: PDFDestination)

Navigates to the specified destination.

func go(to: PDFSelection)

Scrolls to the first character of the specified selection.

func go(to: CGRect, on: PDFPage)

Navigates to the specified rectangle on the specified page.

