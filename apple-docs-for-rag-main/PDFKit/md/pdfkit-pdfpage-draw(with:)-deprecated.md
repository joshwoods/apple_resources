

- PDFKit
- PDFPage
-  draw(with:) Deprecated

Instance Method

# draw(with:)

Draws the page within the specified box.

macOS 10.4–10.12Deprecated

``` source
func draw(with box: PDFDisplayBox)
```

## Mentioned in 

Adding Custom Graphics to a PDF

## Discussion

This method takes into account the page rotation and draws clipped to the specified box. If the page is set to display annotations, this method also draws them. This method does not clear the background. To clear the background before drawing, use doc://com.apple.documentation/documentation/appkit/1473652-nsrectfill with `NSColor` set (typically) to white.

## See Also

### Related Documentation

var displaysAnnotations: Bool

Returns a Boolean value indicating whether annotations are displayed for the page.

### Rendering Pages

func transformContext(for: PDFDisplayBox)

Transforms the current context, given the specified box.

Deprecated

