

- PDFKit
- PDFView
-  documentView 

Instance Property

# documentView

The innermost view used by `PDFView` or by your `PDFView` subclass.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS**

``` source
@MainActor
var documentView: UIView? { get }
```

**macOS**

``` source
@MainActor
var documentView: NSView? { get }
```

## Discussion

The innermost view is the one displaying the visible document pages. This method is useful when converting coordinates from one view to another.

## See Also

### Specializing the View

func layoutDocumentView()

Performs layout of the inner views.

Draw Operations

Draw in a PDF page.

