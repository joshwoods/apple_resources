

- PDFKit
- PDFView
-  draw(\_:to:) 

Instance Method

# draw(\_:to:)

Draw and render a visible page to a context.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+

``` source
@MainActor
func draw(
    _ page: PDFPage,
    to context: CGContext
)
```

## See Also

### Drawing in a PDF Page

func drawPagePost(PDFPage, to: CGContext)

Perform post-page rendering for a page rendered to a context.

