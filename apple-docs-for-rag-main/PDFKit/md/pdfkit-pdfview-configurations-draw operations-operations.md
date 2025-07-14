

- PDFKit
- PDFView
- Configurations
-  Draw Operations 

API Collection

# Draw Operations

Draw in a PDF page.

## Topics

### Drawing in a PDF Page

func draw(PDFPage, to: CGContext)

Draw and render a visible page to a context.

func drawPagePost(PDFPage, to: CGContext)

Perform post-page rendering for a page rendered to a context.

## See Also

### Specializing the View

var documentView: UIView?

The innermost view used by `PDFView` or by your `PDFView` subclass.

func layoutDocumentView()

Performs layout of the inner views.

