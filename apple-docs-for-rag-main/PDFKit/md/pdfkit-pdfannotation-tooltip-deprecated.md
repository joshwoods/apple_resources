

- PDFKit
- PDFAnnotation
-  toolTip Deprecated

Instance Property

# toolTip

Returns text for display as a help tag.

macOS 10.5–10.12Deprecated

``` source
var toolTip: String? { get }
```

## Return Value

A string that contains help tag content, or `NULL` if there is no text associated with the annotation.

## Discussion

This method is equivalent to sending the message `[self contents]`. PDF Kit’s annotation subclasses override this behavior as appropriate. For example, a `PDFAnnotationLink` object displays a URL or page destination for its help tag.

## See Also

### Deprecated Properties

var mouseUpAction: PDFAction?

The action to perform when a user releases the mouse button within an annotation.

Deprecated

