

- PDFKit
- PDFView
-  drawPagePost(\_:to:) 

Instance Method

# drawPagePost(\_:to:)

Perform post-page rendering for a page rendered to a context.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func drawPagePost(
    _ page: PDFPage,
    to context: CGContext
)
```

## See Also

### Drawing in a PDF Page

func draw(PDFPage, to: CGContext)

Draw and render a visible page to a context.

