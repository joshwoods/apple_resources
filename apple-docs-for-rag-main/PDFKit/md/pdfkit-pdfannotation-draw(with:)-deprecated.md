

- PDFKit
- PDFAnnotation
-  draw(with:) Deprecated

Instance Method

# draw(with:)

Draws the annotation on its associated page.

macOS 10.4–10.12Deprecated

``` source
func draw(with box: PDFDisplayBox)
```

Deprecated

Use draw(with:in:) instead.

## Parameters 

`box`  

The bounding box to draw the annotation in.

## Mentioned in 

Adding Custom Graphics to a PDF

## Discussion

The annotation is drawn relative to the origin of `box` in page-space coordinates.

Page space is a 72 dpi coordinate system with the origin at the lower-left corner of the current page.

## See Also

### Related Documentation

func bounds(for: PDFDisplayBox) -> CGRect

Returns the bounds for the specified PDF display box.

### Deprecated Methods

convenience init(bounds: NSRect)

Creates a PDF annotation object.

Deprecated

convenience init(dictionary: [AnyHashable : Any], forPage: PDFPage?)Deprecated

func removeAllAppearanceStreams()Deprecated

