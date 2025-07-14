

- PDFKit
- PDFPage
-  transformContext(for:) Deprecated

Instance Method

# transformContext(for:)

Transforms the current context, given the specified box.

macOS 10.5–10.12Deprecated

``` source
func transformContext(for box: PDFDisplayBox)
```

## Discussion

When transforming the current context, this method takes into account the rotation of the page, as well as the origin of the box with respect to the page’s base coordinate system. This is a convenient method to call within the `PDFView` draw(_:) method or from within a draw method of a `PDFAnnotation` subclass.

## See Also

### Related Documentation

class PDFPage

`PDFPage`, a subclass of `NSObject`, defines methods used to render PDF pages and work with annotations, text, and selections.

### Rendering Pages

func draw(with: PDFDisplayBox)

Draws the page within the specified box.

Deprecated

